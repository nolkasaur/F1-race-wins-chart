# F1 race wins (1950-2021)

**Top 20 number of race wins by drivers from 1950 to 2021**

This chart animates the top 20 number of race wins by drivers from 1950 to 2021. Colors are random (ToDo: make them relevant). Data manually extracted from the respective wikipedia pages of each F1 season (ToDo: recheck the data again to confirm no mistakes).

Compressed demo visualization:

https://user-images.githubusercontent.com/7191666/182831740-82f805bb-005b-4029-bc19-a34a65429071.mp4

https://observablehq.com/d/a44c1c0df7579abb@3068

View this notebook in your browser by running a web server in this folder. For
example:

~~~sh
npx http-server
~~~

Or, use the [Observable Runtime](https://github.com/observablehq/runtime) to
import this module directly into your application. To npm install:

~~~sh
npm install @observablehq/runtime@4
npm install https://api.observablehq.com/d/a44c1c0df7579abb@3068.tgz?v=3
~~~

Then, import your notebook and the runtime as:

~~~js
import {Runtime, Inspector} from "@observablehq/runtime";
import define from "a44c1c0df7579abb";
~~~

To log the value of the cell named “foo”:

~~~js
const runtime = new Runtime();
const main = runtime.module(define);
main.value("foo").then(value => console.log(value));
~~~
