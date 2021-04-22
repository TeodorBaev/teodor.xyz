---
title: "CPU fan monitoring and alert on failure"
date: 2021-04-21T18:51:23+03:00
draft: true
toc: false
images:
tags:
  - scripts
---

## Introduction

Faulty fan can lead to system failure and throthe of the preformance. Here we are going to write a small script that will check the fan speed.

## Software needed
Keeping things simple we will use "sensors" to get the needed information and parse it with "awk". 

To check if you have sensors install open a terminal and type "sensors"

```js
/// <reference lib="WebWorker"/>

var _self = (typeof window !== 'undefined')
	? window   // if in browser
	: (
		(typeof WorkerGlobalScope !== 'undefined' && self instanceof WorkerGlobalScope)
		? self // if in worker
		: {}   // if in node js
	);
```
