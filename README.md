## Kud venkat links
* http://csharp-video-tutorials.blogspot.com/2017/06/angular-2-tutorial-for-beginners_12.html
* http://csharp-video-tutorials.blogspot.com/2017/10/angular-cli-tutorial-for-beginners.html
* http://csharp-video-tutorials.blogspot.com/2017/12/angular-crud-tutorial.html
* http://csharp-video-tutorials.blogspot.com/2018/09/angular-6-tutorial-for-beginners.html


## Angular Topics

### Introduction
``````````````````
Angular 1 released in oct 2010
Angular 2 is 5 times faster than 1
Has mobile support
Component based development
Built using typscript which is free and open source language developed by Microsoft
```````````````````

### What is ECMAscript
```````````````````````
Javascript language standard
Most modern browsers support ECMAscript5
The browser support for ECMAscript6 is still incomplete
ECMAscript6 is oficially known as ECMAscript 2015
Transpilers compile code in the latest version into older versions(use to compile ES6 to ES5)
Babel is one of the transpiler
````````````````````````

### What is Typescript
`````````````````````````
Superset of Javascript
Transpilation compiles typescript to Javascript
`````````````````````````

### Other Topics
`````````````````````````
Component
	Decorator that makes a class as an angular component

template, templateUrl
nested component
styles, styleUrl
One way data binding:
	From component to view template - interpolation, property binding, attribute binding etc.
interpolation:
	converts to property binding
	To concatinate strings - {{}}
property binding
	any(string or non-string) values can be bind
	[x]='x'
attribute binding
	[attr.colspan]="columnspan"
class binding
	[class]="classesToApply"
	[class.boldClass]="true"
	[ngClass] = "addClasses()"
style binding
	[style.font-weight]="Bold"
	[style.font-size.px]='20'
	[ngstyle]="addstyles()"
event binding
	(click)="onclick()"
two way binding(combination of property binding and event binding)[()]
	[(ngModel)]=''
	import { FormsModule } from '@angular/forms';
*ngIf
*ngFor
	<tr *ngFor='let employee of employees; trackBy:trackByEmpCode; 
	let i= index; let isFirst = first; let isLast = last; let isEven = even; let isOdd = odd''>
Pipes
	uppercase, lowercase, percent, currency, date
	custom pipes
	import { Pipe, PipeTransform } from '@angular/core';
	@Pipe({name: 'x'})
Component input properties
	@Input (from container component to Nested component)
Component output properties
	@Output
	EventEmitter
Interfaces
Life Cycle Hook
	OnInit, ngOnInit
	OnChanges, ngOnChanges, SimpleChanges
	OnDestroy, ngOnDestroy
Services
	@Injectable
	Providers(component level, module level)
Http Service
	HttpModule
	Http, Response
	Observable
	map
	subscribe(OnNext, onError, onCompleted)
Http error handliing
	import { RouterModule, Routes } from '@angular/router';	
	RouterModule.forRoot(routes)
	routerLinkActive
	<a routerLink="x">
	<router-outlet/>
	[routerLink]="[]"
Singleton, dependency Injection
root module and feature module
router navigate
	router.navigate
ActivatedRoute
	activatedRoute.snapshot.params['code'];	
promises vs observable
	map, forEach, filter, reduce, retry, retryWhen
	then() instead of subscribe
	unsubscribe
	ISubscription
`````````````````````````````

### Import statements
````````````````````````
import {Component, NgModule, input, output, EventEmitter, Pipe, PipeTransform} from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { FormsModule } from '@angular/forms';
import { Pipe, PipeTransform } from '@angular/core';
import { HttpModule } from '@angular/http';
import { RouterModule, Routes } from '@angular/router';
````````````````````````
