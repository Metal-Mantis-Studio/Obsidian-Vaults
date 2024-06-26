---
tags: Angular, Dependency-Injection, Services, Components, Modules
---
[Dependency Injection](https://angular.io/guide/dependency-injection)
![[Pasted image 20230730224916.png]]

When a dependency is requested, the injector checks its registry for an existing and available instance of that dependency. If one exists, it'll use that otherwise create a new one. During Angular's Bootstrap process, a root injector is created. When an injectable service is created, all dependencies must be resolved before the service is returned to Angular.

```TS
@Injectable()
class ZooManagementService {}
```

## Injecting at the [[Components]] level
Dependencies injected at the component level will have a one-to-one with that specific instance of that component. With each new instance of that component, a corresponding instance of the dependency will be created.
```TS
@[Component]({ 
	selector: 'zoo-management', 
	template: '...', 
	providers: [ZooManagementService]
})
class ZooManagementComponent {}
```

## Injecting at the [[Modules]] level
Injecting a dependency at the module level creates a single instance of that service at the root level meaning that all components, directives and pipes within this module will utilise a singular instance of that dependency.
```TS
@[NgModule]({ 
	declarations: [ZooManagementComponent] 
	providers: [ZooManagementService] 
})
class ZooManagementModule {}
```

## Creating Root [[Services]]
[Injectable Services](https://angular.io/guide/creating-injectable-service)
Services with the `@Injectable()` decorator will be visible throughout the application
```TS
@Injectable({ providedIn: 'root' })
class ZooManagementService {}
```

This Angular CLI will generate a generic service template
```TS
ng generate service path1/path2/filename
```


## Injecting Dependencies

Via a constructor
```TS
@Component({})
class ZooManagementModule {
	constructor(
		private zooManagementService: ZooManagementService
	) {}
}
```

Via the inject method
```TS
@Component({})
class ZooManagementModule {
	private zooManagementService: ZooManagementService;
}
```

## Injection Tokens
[Defining Dependency Injectors](https://angular.io/guide/dependency-injection-providers)