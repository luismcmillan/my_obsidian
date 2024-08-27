[[TypeScript/TypeScript]]
[[Final]]
```TypeScript
import { Injectable } from '@angular/core';

export class Finalvariable{
	number_variable: ReadOnlySet<number> = new Set([0]);
	string_variable: ReadOnlySet<string> = new Set(['\u001b']);
	
	private getValue():number {
		return [...this.number_variable][0];
	}
}
```