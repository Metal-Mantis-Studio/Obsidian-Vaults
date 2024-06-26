---
tags: Angular, BehaviourSubject, Subscription
---

Async [[Pipes]]
```
| async
```

### BehaviourSubject
```TS
Products$ : BehaviorSubject<IProduct[]>; 
	private subscriptions = Subscription[] = [];

	constructor() {
		this.Products$ = new BehaviorSubject<IProduct[]>(this.Products);
	}
  
   AddProduct(p: IProduct): void{
    this.Products.push(p);
    this.Products$.next(this.Products);
   }

   ngOnDestroy(): void {
	   this.subscriptions.add(
		   this.productSubscription$$.subscribe(products => {
			   console.log(`Products: `, products)
		   })
		)
   }

   ngOnDestroy(): void {
		this.subscriptions.unsubscribe();
   }
```

### Unsubscribe on destroy
Subscriptions will remain even after a class is destroyed so it's best practise to use `this.subscriptions.unsubscribe()`. 

