# Typescript-notes-in-Roman-urdu
Typescript:

Typescript kya hai?
Typescript ek programming language hai jo JavaScript par based hai. Iski maqsad JavaScript ko robust, scalable, aur maintainable banane ka hai. Typescript mein static typing hoti hai, jisse code mein errors kam hote hain aur development process mein asaan hoti hai.

Typescript Kaise Likha Jaye:

1. Typescript Install Karna:
   Typescript likhne ke liye sabse pehle Node.js aur npm install karna zaroori hai. Terminal mein `npm install -g typescript` command se Typescript ko global install kar sakte hain.

2. Typescript File Banayein:
   Typescript files `.ts` extension ke hote hain. Aap ek text editor ya Integrated Development Environment (IDE) jaise VSCode mein `.ts` file create kar sakte hain.

3. Code Likhein:
   Typescript mein code likhne ke liye JavaScript ke tareeqe ke sath sath, aapko Typescript ke features ka bhi istemal karna hoga jaise ke types, interfaces, enums, etc.
   ```typescript
   // Example: Typescript mein variable declaration
   let naam: string = "kiran";
   ```

4. Compile Karna:
   Typescript code ko JavaScript mein compile karne ke liye terminal mein `tsc filename.ts` command use karein. Isse aapko ek `.js` file milega.
   ```bash
   tsc filename.ts
   ```

5. JavaScript Run Karna:
   Ab aap apne compiled JavaScript file ko run kar sakte hain, jaise ke `node filename.js`.
   ```bash
   node filename.js
   ```

Typescript Sikhein:

1. Official Documentation:
   Typescript ki official documentation ko parhna shuru karein. Isme aapko language ke har pehlu ka pata chalega.

2. Online Tutorials:
   Internet par bohat se tutorials mojood hain jo step-by-step guide karte hain. Udemy, Codecademy, aur FreeCodeCamp jaise platforms par aapko Typescript ke tutorials mil sakte hain.

3. Practice Projects:
   Apne learning ko reinforce karne ke liye small projects shuru karein. Isse aapko real-world application of concepts samajh aayega.

4. Read Code:
   Open source projects ya dusre developers ke code ko padh kar aap apni understanding ko mazeed barha sakte hain.

Typescript Ke Taqatwar Pehlu:

1. Fundamentals (Bunyadi Tawunat):
   Typescript ke bunyadi concepts mein variables, data types, loops, conditions, functions, aur classes shamil hain.
   - Variables (Variables): Typescript mein variables declare karte waqt unke data types specify kiye jate hain, jaise ke `let naam: string = "kiran";`.
   - Data Types (Data Qisamain): Typescript mein data types include hain string, number, boolean, array, tuple, enum, any, void, etc.
   - Loops (Loops): Typescript mein for, while, aur do-while loops hote hain.
   - Conditions (Shartain): If-else statements aur switch statements typescript mein istemal ho sakte hain.
   - Functions (Functions): Functions Typescript mein JavaScript ke functions ke sath sath additional features jaise default parameters, rest parameters, aur arrow functions ke sath aate hain.

2. Advanced Types (Takmeel Shuda Qisamain):
   Typescript mein advanced types jaise ke union types, intersection types, generics, conditional types, mapped types, etc., ko samajhna important hai.

3. Modules (Module):
   Large-scale applications ke liye module system use hota hai. Typescript mein aapko module system ke liye `import` aur `export` keywords milte hain.

4. Decorators (Sajjaad):
   Decorators ek powerful feature hain jo Typescript ko object-oriented programming mein aur bhi flexible banate hain.

5. Asynchronous Programming (Be Rabti Programming):
   Typescript mein asynchronous programming ke liye `async/await` syntax ka istemal hota hai. Promises bhi ek important concept hai.

6. Frameworks (Framework):
   Popular frontend frameworks jaise ke Angular, React, aur Vue.js Typescript ke sath integrate ho sakte hain.

Yeh kuch basics hain jo aapko Typescript ke istemal aur sikhnay mein madad kareinge. Har level par practice aur real-world projects ka hissa banayein taake aap apni skills ko improve kar sakein.



Basic types


TypeScript k basic types ye hain:

- **boolean**: true ya false ki values rakhne wale types. Masalan, `let isDone: boolean = false;`
- **number**: integer ya floating point numbers rakhne wale types. Masalan, `let decimal: number = 6;`
- **string**: text ya characters rakhne wale types. Masalan, `let color: string = "blue";`
- **array**: ek hi type k values ka collection rakhne wale types. Masalan, `let list: number[] = [1, 2, 3];`
- **tuple**: mukhtalif types k values ka fixed size ka collection rakhne wale types. Masalan, `let x: [string, number] = ["hello", 10];`
- **enum**: predefined constants ka set rakhne wale types. Masalan, `enum Color {Red, Green, Blue};`
- **any**: kisi bhi type ki value rakh sakte hain. Masalan, `let notSure: any = 4;`
- **void**: koi value na rakhne wale types. Masalan, `function warnUser(): void { console.log("Warning!"); }`
- **null** aur **undefined**: koi value na hone wale types. Masalan, `let u: undefined = undefined; let n: null = null;`
- **never**: kabhi return na hone wale types. Masalan, `function error(message: string): never { throw new Error(message); }`
- **object**: non-primitive values rakhne wale types. Masalan, `let user: object = {name: "Ali", age: 25};`




Interface

TypeScript interface ka matlab hai kisi object ki shakal aur rawaiya ko tareef karna, baghair kisi implementation ki tafseelat ko bataye. Ek interface mein properties, methods, aur index signatures ho sakte hain, sath hi sath optional aur readonly modifiers bhi. Ek interface dusre interfaces ya classes se extend ya inherit bhi kar sakta hai. Ek interface ko object, function, class, ya constructor ki type ko bayan karne ke liye istemal kiya ja sakta hai.

TypeScript interface ke kuch khaas khobiyan yeh hain:

- Interface ka naam hamesha capital letter se shuru hota hai, jaise `Person`, `SquareConfig`, etc.
- Interface mein property ka naam ke baad colon (`:`) lagana zaroori hai, jaise `name: string;`, `width?: number;`, etc.
- Interface mein property ke baad semicolon (`;`) lagana zaroori hai, jaise `name: string;`, `width?: number;`, etc.
- Interface mein method ka naam ke baad parantheses (`()`) lagana zaroori hai, jaise `greet(): void;`, `measureTirePressure(): void;`, etc.
- Interface mein method ke baad semicolon (`;`) lagana zaroori hai, jaise `greet(): void;`, `measureTirePressure(): void;`, etc.
- Interface mein optional property ke naam ke baad question mark (`?`) lagana zaroori hai, jaise `age?: number;`, `width?: number;`, etc.
- Interface mein readonly property ke naam se pehle `readonly` keyword lagana zaroori hai, jaise `readonly name: string;`, `readonly length: number;`, etc.
- Interface mein index signature ke andar square brackets (`[]`) lagana zaroori hai, jaise `[key: string]: any;`, `[index: number]: string;`, etc.
- Interface mein function type ke andar parantheses (`()`) aur arrow (`=>`) lagana zaroori hai, jaise `(name: string) => void;`, `(a: number, b: number) => number;`, etc.
- Interface mein constructor type ke andar `new` keyword aur parantheses (`()`) lagana zaroori hai, jaise `new (name: string, age?: number): Person;`, `new (length: number, width: number): Rectangle;`, etc.


Classes 
TypeScript class ka matlab hai kisi object ki shakal aur rawaiya ko tareef karna, sath hi sath uski implementation ki tafseelat ko bhi batana. Ek class mein properties, methods, constructors, access modifiers, inheritance, aur static members ho sakte hain. Ek class ko object, function, class, ya constructor ki type ko bayan karne ke liye istemal kiya ja sakta hai.

TypeScript class ke kuch khaas khobiyan yeh hain:

- Class ka naam hamesha capital letter se shuru hota hai, jaise `Employee`, `Rectangle`, etc.
- Class mein property ka naam ke baad colon (`:`) lagana zaroori hai, jaise `name: string;`, `width: number;`, etc.
- Class mein property ke baad semicolon (`;`) lagana zaroori hai, jaise `name: string;`, `width: number;`, etc.
- Class mein method ka naam ke baad parantheses (`()`) lagana zaroori hai, jaise `greet(): void;`, `area(): number;`, etc.
- Class mein method ke andar curly braces (`{}`) lagana zaroori hai, jaise `greet(): void { console.log("Hello"); }`, `area(): number { return this.width * this.height; }`, etc.
- Class mein constructor ka naam hamesha `constructor` hona chahiye, aur uske baad parantheses (`()`) aur curly braces (`{}`) lagana zaroori hai, jaise `constructor(name: string, age: number) { this.name = name; this.age = age; }`, `constructor(length: number, width: number) { this.length = length; this.width = width; }`, etc.
- Class mein property ya method ke naam se pehle access modifier lagana mumkin hai, jaise `public`, `private`, `protected`, etc. Agar koi access modifier nahi diya gaya, to default `public` hota hai.
- Class mein property ya method ke naam se pehle `static` keyword lagana mumkin hai, jaise `static count: number;`, `static getInstance(): Singleton;`, etc. Static members sirf class ke naam se access kiye ja sakte hain, aur class ke instances se nahi.
- Class mein property ya method ke naam se pehle `abstract` keyword lagana mumkin hai, jaise `abstract name: string;`, `abstract greet(): void;`, etc. Abstract members sirf abstract classes mein ho sakte hain, aur unki implementation derived classes mein di jati hai.
- Class ko dusre class se extend kar sakte hain, jaise `class Manager extends Employee { ... }`, `class Square extends Rectangle { ... }`, etc. Extend karne se class ko base class ke sare members inherit ho jate hain, aur unhe override bhi kar sakte hain.
- Class ko ek ya zyada interfaces se implement kar sakte hain, jaise `class Employee implements Person, Comparable<Employee> { ... }`, `class Rectangle implements Shape, Printable { ... }`, etc. Implement karne se class ko interface ke sare members implement karna parta hai.


Functions

TypeScript functions kay baray mein complete details yeh hain:

- TypeScript functions ko function keyword kay sath declare kiya jata hai, jaisa kay JavaScript mein hota hai. Lekin TypeScript mein function kay parameters aur return type ko bhi specify karna parta hai. Masalan, `function name(parameter: type, parameter:type,...): returnType { // do something }` ka matlab hai “aik function jis ka naam name hai, jis kay kuch parameters hain, jin ki type batayi gayi hai, jo aik value return karta hai, jis ki type batayi gayi hai”.
- TypeScript functions ko mukhtalif tareeqon se declare kiya ja sakta hai, jaisa kay JavaScript mein hota hai. Masalan, function expressions, arrow functions, anonymous functions, etc. In sab mein function kay parameters aur return type ko specify karna zaroori hai. Masalan, `let add = function(x: number, y: number): number { return x + y; }` ya `let multiply = (x: number, y: number): number => x * y;` ya `function greet(name: string): void { console.log("Hello, " + name); }`.
- TypeScript functions mein optional parameters, default parameters, rest parameters, aur spread parameters bhi istemal kiye ja saktay hain, jaisa kay JavaScript mein hota hai. Optional parameters ko `?` kay sath denote kiya jata hai. Masalan, `function printName(firstName: string, lastName?: string): void { // do something }`. Default parameters ko `=` kay sath assign kiya jata hai. Masalan, `function printName(firstName: string, lastName = "Smith"): void { // do something }`. Rest parameters ko `...` kay sath denote kiya jata hai. Masalan, `function sum(...numbers: number[]): number { // do something }`. Spread parameters bhi `...` kay sath denote kiye jatay hain, lekin function call mein istemal hotay hain. Masalan, `let numbers = [1, 2, 3]; sum(...numbers);`.
- TypeScript functions mein function overloading bhi kiya ja sakta hai, yani aik hi function kay liye mukhtalif signatures define kiye ja saktay hain. Lekin is kay liye function implementation mein aik generic signature hona chahiye, jo har signature kay liye kaam kar sakay. Masalan, `function add(x: string, y: string): string; function add(x: number, y: number): number; function add(x: any, y: any): any { return x + y; }`.
- TypeScript functions mein generic functions bhi banaye ja saktay hain, yani aisi functions jo mukhtalif types kay input aur output kay sath kaam kartay hain, type parameters aur type constraints istemal kartay hain. Masalan, `function firstElement<T>(arr: T[]): T { return arr[0]; }`.


Generic of Typescript 

TypeScript kay generic kay baray mein complete details yeh hain:
- Generic aik tarah kay placeholder ya type parameters hain, jo TypeScript mein reusable components bananay kay liye istemal hotay hain. Yeh aap ko aisa function ya class bananay ki ijazat detay hain, jis mein aap data types specify nahi kartay, jab tak kay woh function ya class call na ho jaye. Generic ka maqsad yeh hai kay aap apnay component ko aisi type kay data kay sath istemal kar sakain, jo aap chahtay hain, aur us type ko function ya class mein enforce kar sakain¹².
- Generic ko `<T>` ki surat mein likha jata hai, jahan T aik type variable hai, jo kisi bhi type ko represent kar sakta hai. Aap T ki jagah koi bhi naam istemal kar saktay hain, lekin conventionally T, U, V, etc. istemal hotay hain. Masalan, `function identity<T>(arg: T): T` aik generic function hai, jo kisi bhi type ka argument lay kar usi type ka value return karta hai¹.
- Generic ko function, type, class, aur interface mein istemal kiya ja sakta hai. Function mein generic ko parameter list kay pehlay likha jata hai. Masalan, `function firstElement<T>(arr: T[]): T` aik generic function hai, jo kisi bhi type ki array ka pehla element return karta hai¹. Type mein generic ko type name kay baad likha jata hai. Masalan, `type Box<T> = { value: T }` aik generic type hai, jo kisi bhi type ki value rakhnay wala object hai¹. Class mein generic ko class name kay baad likha jata hai. Masalan, `class Stack<T> { items: T[]; push(item: T) { this.items.push(item); } pop(): T { return this.items.pop(); } }` aik generic class hai, jo kisi bhi type kay items ko stack mein rakhnay wali hai¹. Interface mein generic ko interface name kay baad likha jata hai. Masalan, `interface Comparable<T> { compareTo(other: T): number; }` aik generic interface hai, jo kisi bhi type kay objects ko compare karnay wali hai¹.
- Generic mein aap type constraints bhi istemal kar saktay hain, jo aap kay type variable ko kisi specific type ya interface kay sath bound kartay hain. Is say aap type variable kay properties ya methods ko access kar saktay hain. Type constraints ko `extends` keyword kay sath likha jata hai. Masalan, `function getProperty<T, K extends keyof T>(obj: T, key: K) { return obj[key]; }` aik generic function hai, jo kisi bhi type kay object ka koi bhi property return karta hai, lekin is mein K type variable T type kay keys mein say hona chahiye¹.
- Generic mein aap conditional types bhi istemal kar saktay hain, jo aik type ko kisi condition kay mutabiq define kartay hain. Conditional types ko `extends` aur `?` kay sath likha jata hai. Masalan, `type NonNullable<T> = T extends null | undefined ? never : T` aik conditional type hai, jo kisi bhi type ko null ya undefined say exclude kar deta hai¹.
- Generic mein aap mapped types bhi istemal kar saktay hain, jo aik type kay properties ko iterate kartay hain aur un ko modify kartay hain. Mapped types ko `in` keyword kay sath likha jata hai. Masalan, `type Readonly<T> = { readonly [P in keyof T]: T[P] }` aik mapped type hai, jo kisi bhi type kay object kay tamam properties ko readonly bana deta hai¹.



.
Inference

TypeScript mein type inference aik aisi khobi hai, jo TypeScript compiler ko aik variable ya expression ki type khud ba khud maloom karne ki ijazat deti hai. Is ka matlab yeh hai kay aap ko har variable aur expression ki type khud se batane ki zaroorat nahi hoti¹.

TypeScript mein type inference mukhtalif jagahon par istemal hota hai, jahan type annotation mojood nahi hota. Masalan, jab aap variables ko initialize kartay hain, parameter default values set kartay hain, ya function return types tay kartay hain. TypeScript behtareen common type algorithm istemal karta hai, jo mukhtalif variables kay darmiyan compatible types ko select karta hai².

TypeScript mein type inference doosri taraf bhi kaam karta hai, kuch cases mein. Is ko contextual typing kehtay hain. Contextual typing tab hoti hai, jab aik expression ki type us ki location ki wajah se imply ho jati hai. Masalan, agar aap aik function ko aik interface kay property mein assign kartay hain, to TypeScript us function kay parameter aur return type ko us interface kay mutabiq infer kar lega².

TypeScript mein type inference kay baray mein complete details yeh hain:

- Type inference kay liye TypeScript aik variable ya expression ki initial value ko dekhta hai, aur us ki type ko allocate karta hai. Masalan, `let x = 3;` mein TypeScript x ki type ko number bana dega¹.
- Type inference kay liye TypeScript aik variable ya expression ki context ko bhi dekhta hai, aur us ki type ko us kay sath match karta hai. Masalan, `let x: string; x = 3;` mein TypeScript x ki type ko string samjhay ga, aur 3 ko assign karnay par error day ga¹.
- Type inference kay liye TypeScript aik variable ya expression ki usage ko bhi dekhta hai, aur us ki type ko us kay sath compatible karta hai. Masalan, `let x; x = 3; x = "hello";` mein TypeScript x ki type ko any bana dega, aur 3 ya "hello" ko assign karnay par koi error nahi day ga¹.
- Type inference kay liye TypeScript aik variable ya expression ki surrounding code ko bhi dekhta hai, au  us ki type ko us kay sath infer karta hai. Masalan, `let x = [0, 1, null];` mein TypeScript x ki type ko `(number | null)[]` bana dega, kyun kay array mein number aur null dono types hain².
- Type inference kay liye TypeScript aik variable ya expression ki expected type ko bhi dekhta hai, aur us ki type ko us kay sath narrow karta hai. Masalan, `function isFish(pet: Fish | Bird): pet is Fish { return (pet as Fish).swim !== undefined; }` mein TypeScript pet ki type ko Fish ya Bird samjhay ga, aur isFish kay andar pet ki type ko Fish hi samjhay ga².




Advance Types 

TypeScript kay advanced types aisi types hain, jo aap ko complex type definitions bananay mein madad kartay hain. Advanced types mein union types, intersection types, conditional types, mapped types, aur dosray features shamil hain¹².

Advanced types kay baray mein complete details yeh hain:

- Union types aisi types hain, jo aik variable ya expression kay liye mukhtalif types ki possibility ko model kartay hain. Union types ko `|` kay sath likha jata hai. Masalan, `let x: number | string;` ka matlab hai kay x aik number ya string ho sakta hai¹.
- Intersection types aisi types hain, jo mukhtalif types ko aik mein mila detay hain. Intersection types ko `&` kay sath likha jata hai. Masalan, `let y: { name: string } & { age: number };` ka matlab hai kay y aik object hai, jis mein name aur age dono properties hain¹.
- Conditional types aisi types hain, jo aik type ko kisi condition kay mutabiq define kartay hain. Conditional types ko `extends` aur `?` kay sath likha jata hai. Masalan, `type NonNullable<T> = T extends null | undefined ? never : T` aik conditional type hai, jo kisi bhi type ko null ya undefined say exclude kar deta hai¹.
- Mapped types aisi types hain, jo aik type kay properties ko iterate kartay hain aur un ko modify kartay hain. Mapped types ko `in` keyword kay sath likha jata hai. Masalan, `type Readonly<T> = { readonly [P in keyof T]: T[P] }` aik mapped type hai, jo kisi bhi type kay object kay tamam properties ko readonly bana deta hai¹.
- Index types aisi types hain, jo aik type kay keys ya values ko access kartay hain. Index types ko `keyof` aur `[]` kay sath likha jata hai. Masalan, `type K = keyof { name: string, age: number }` aik index type hai, jo "name" ya "age" ho sakta hai¹.
- Literal types aisi types hain, jo aik specific value ko represent kartay hain. Literal types ko string, number, boolean, aur enum literals kay sath likha jata hai. Masalan, `type Direction = "north" | "south" | "east" | "west"` aik literal type hai, jo kisi aik direction ko represent karta hai¹.
- Template literal types aisi types hain, jo string literals ko concatenate ya manipulate kartay hain. Template literal types ko backticks kay sath likha jata hai. Masalan, `type World = "world"; type Greeting = `Hello ${World}`` aik template literal type hai, jo "Hello world" ko represent karta hai¹.






Enums in Typescript 

TypeScript kay Enums kay baray mein complete details yeh hain:

- Enums aik aisi feature hain, jo TypeScript nay JavaScript mein shamil ki hai, jo aap ko constant values ka aik set define karnay mein asani deti hain. Har aik constant value ko enum ka aik member kehtay hain. Enums aap ko aisi properties ya values set karnay mein madad kartay hain, jo sirf aik makhsoos tadaad kay mumkin values ho sakti hain. Aik aam misal hai, aik deck of playing cards mein aik card ka suit value. Har card jo nikala jaye ga, ya to club, ya diamond, ya heart, ya spade ho ga; in charon kay ilawa koi aur suit value mumkin nahi hai, aur yeh mumkin values badalnay kay liye bhi nahi hain. Is liye, enum aik efficient aur clear tareeqa hai, card kay suit kay mumkin values ko describe karnay ka¹².
- Enums ko enum keyword kay sath define kiya jata hai. Masalan, `enum Suit { Club, Diamond, Heart, Spade }` aik enum hai, jo card kay suit ko represent karta hai¹.
- Enums ko numeric aur string dono tarah kay base par banaya ja sakta hai. Numeric enums mein har member ko aik number assign hota hai, jo default tor par zero say shuru hota hai, aur har member par aik increment hota hai. Yeh tab mufeed hota hai, jab aap ko member values ki ahmiyat nahi hoti, balkay aap ko sirf yeh zaroori hota hai kay har value dosri values say distinct ho. String enums mein har member ko aik string assign hota hai, jo us member ka naam hi ho sakta hai. Yeh tab mufeed hota hai, jab aap ko member values ki readability aur serialization ki zaroorat hoti hai¹.
- Enums ko heterogeneous bhi banaya ja sakta hai, yani numeric aur string members ko mix kar diya ja sakta hai, lekin yeh aam tor par acha nahi samjha jata¹.
- Enums ko computed aur constant members bhi banaya ja sakta hai. Constant members woh hain, jo compile time par evaluate ho jatay hain, jaisa kay literal values, ya dosray constant enum members. Computed members woh hain, jo runtime par evaluate hotay hain, jaisa kay function calls, ya arithmetic expressions. Computed members ko initialize karna zaroori hota hai, warna error aata hai¹.
- Enums ko reverse mapping bhi kiya ja sakta hai, yani aap aik member value say us ka naam bhi maloom kar saktay hain. Yeh sirf numeric enums kay liye mumkin hai. Masalan, `let suitName = Suit[2];` say aap ko "Heart" milay ga¹.
- Enums ko const enums bhi banaya ja sakta hai, yani aap enum kay samnay const keyword laga saktay hain. Is say aap ka code mein enum ka object nahi banta, balkay har member ka value directly replace ho jata hai. Yeh aap kay code ko optimize karnay mein madad karta hai, lekin is kay sath aap reverse mapping nahi kar saktay¹.





Modules of Typescript.
TypeScript kay modules kay baray mein complete details yeh hain:

- Modules aik aisi feature hain, jo TypeScript nay JavaScript mein shamil ki hai, jo aap ko aap kay code ko alag alag, reusable pieces mein organize karnay mein asani deti hain. Aik module aik file hai, jo related code, jaisa kay functions, classes, ya interfaces, ko rakhta hai¹.
- Modules apni apni scope mein execute hotay hain, global scope mein nahi. Is ka matlab yeh hai kay modules mein declare kiye gaye variables, functions, classes, etc. module kay bahir nazar nahi aatay, jab tak kay woh explicitly export na kiye jayen. Isi tarah, kisi dosray module say export kiye gaye variable, function, class, interface, etc. ko istemal karnay kay liye import karna parta hai¹.
- Modules ko import aur export kay syntax kay sath define kiya jata hai. Import syntax aik module say kisi specific member ko import karnay kay liye istemal hota hai. Masalan, `import { helloWorld } from "./hello.js";` aik module say helloWorld function ko import karta hai¹. Export syntax aik module mein kisi member ko export karnay kay liye istemal hota hai. Masalan, `export function helloWorld() { console.log("Hello, world!"); }` aik module mein helloWorld function ko export karta hai¹.
- Modules ko default export aur named export dono tarah kay tareeqon se export kiya ja sakta hai. Default export aik module mein sirf aik hi member ko export karta hai, jo module kay default member hota hai. Default export ko import karnay kay liye curly braces ki zaroorat nahi hoti. Masalan, `export default function helloWorld() { console.log("Hello, world!"); }` aik module mein helloWorld function ko default export karta hai, jo `import helloWorld from "./hello.js";` say import kiya ja sakta hai¹. Named export aik module mein aik say zyada members ko export karta hai, jo module kay naam say pehchanay jatay hain. Named export ko import karnay kay liye curly braces ki zaroorat hoti hai. Masalan, `export function helloWorld() { console.log("Hello, world!"); } export function goodbyeWorld() { console.log("Goodbye, world!"); }` aik module mein do functions ko named export karta hai, jo `import { helloWorld, goodbyeWorld } from "./hello.js";` say import kiye ja saktay hain¹.
- Modules ko mukhtalif tareeqon se resolve kiya ja sakta hai, yani aik module kay naam ya path ko aik file kay sath kaisay map kiya jata hai. TypeScript mein do types kay module resolution hain: classic aur node. Classic module resolution aik relative path ko aik relative file kay sath map karta hai, aur aik non-relative path ko aik global file kay sath map karta hai. Node module resolution aik relative path ko aik relative file kay sath map karta hai, aur aik non-relative path ko node_modules folder mein dhoondta hai¹.
- Modules ko mukhtalif module output targets kay liye compile kiya ja sakta hai, yani aik module kay emitted JavaScript code ki format kaisi honi chahiye. TypeScript mein kuch common module output targets yeh hain: commonjs, amd, system, umd, es2015, es2020, etc. In mein say commonjs aur es2015 zyada istemal hotay hain. Commonjs format node.js kay liye mufeed hai, jo require aur module.exports syntax istemal karta hai. Es2015 format web browsers kay liye mufeed hai, jo import aur export syntax istemal karta hai¹.


Namespaces 


TypeScript kay Namespaces kay baray mein complete details yeh hain:

- Namespaces aik aisi feature hain, jo TypeScript nay JavaScript mein shamil ki hai, jo aap ko code ko aik naam wali container mein rakhnay mein asani deti hain. Yeh code ko organize karnay ka aik tareeqa hai aur naam takrao say bachnay mein madad karta hai. Namespaces mein aap functions, classes, interfaces, ya variables ko rakh saktay hain, jo aik ya zyada related functionalities ko support kartay hain¹².
- Namespaces ko namespace keyword kay sath define kiya jata hai. Masalan, `namespace Validation { // code related to validation }` aik namespace hai, jo validation kay mutaliq code ko rakhta hai¹.
- Namespaces mein declare kiye gaye members ko export karna parta hai, agar aap un ko namespace kay bahir istemal karna chahtay hain. Export kay liye aap export keyword istemal kartay hain. Masalan, `namespace Validation { export interface StringValidator { // code for string validator } }` mein StringValidator interface ko export kiya gaya hai, ta kay namespace kay bahir bhi istemal ho sakay¹.
- Namespaces ko import karnay kay liye aap namespace kay naam ko dot notation kay sath istemal kartay hain. Masalan, `let validator: Validation.StringValidator;` mein Validation namespace say StringValidator interface ko import kiya gaya hai¹.
- Namespaces ko multiple files mein bhi span kiya ja sakta hai, yani aap aik namespace ko alag alag files mein define kar saktay hain, aur phir un ko aik file mein mila saktay hain. Is kay liye aap outFile option istemal kartay hain, jo aap kay files ko aik hi file mein concatenate kar deta hai. Masalan, `tsc --outFile sample.js Validation.ts LettersOnlyValidator.ts ZipCodeValidator.ts Test.ts` command say aap Validation, LettersOnlyValidator, ZipCodeValidator, aur Test files ko aik hi file mein mila saktay hain¹.
- Namespaces ko nested bhi banaya ja sakta hai, yani aap aik namespace kay andar dosra namespace define kar saktay hain. Is say aap code ko aur zyada organize kar saktay hain. Masalan, `namespace Shapes { export namespace Polygons { export class Triangle { // code for triangle } export class Square { // code for square } } }` mein Shapes namespace kay andar Polygons namespace define kiya gaya hai, jo Triangle aur Square classes ko export karta hai¹.
- Namespaces ko modules kay sath bhi istemal kiya ja sakta hai, yani aap aik module mein aik namespace define kar saktay hain, aur phir us namespace ko import kar kay istemal kar saktay hain. Is say aap code ko modularize kar saktay hain. Masalan, `export namespace Shapes { export class Circle { // code for circle } }` mein Shapes namespace ko aik module mein export kiya gaya hai, jo Circle class ko export karta hai. Is namespace ko aap `import * as shapes from \"./shapes\"; let c = new shapes.Shapes.Circle();` say import kar kay istemal kar saktay hain¹.








Decorators.

TypeScript kay decorators kay baray mein complete details yeh hain:
- Decorators aik aisi feature hain, jo TypeScript nay JavaScript mein shamil ki hai, jo aap ko classes, methods, properties, aur parameters ko decorate karnay mein asani deti hain. Decorators say aap in elements ki behavior ko observe, modify, ya replace kar saktay hain. Decorators ko `@` symbol kay sath likha jata hai, jis kay baad aik function ka naam hota hai, jo runtime par us element kay baray mein information lay kar execute hota hai¹².
- Decorators ko class, method, accessor, property, aur parameter kay liye istemal kiya ja sakta hai. Class decorator aik class declaration ko decorate karta hai, aur us class kay constructor function ko modify kar sakta hai. Method decorator aik method declaration ko decorate karta hai, aur us method kay descriptor ko modify kar sakta hai. Accessor decorator aik accessor declaration ko decorate karta hai, aur us accessor kay descriptor ko modify kar sakta hai. Property decorator aik property declaration ko decorate karta hai, aur us property kay descriptor ko modify kar sakta hai. Parameter decorator aik parameter declaration ko decorate karta hai, aur us parameter kay metadata ko modify kar sakta hai¹.
- Decorators ko aik say zyada bhi lagaya ja sakta hai, yani aap aik element ko multiple decorators say decorate kar saktay hain. Jab aap aisa kartay hain, to decorators ki evaluation order bottom-to-top hoti hai, aur execution order top-to-bottom hoti hai. Masalan, `@ f () @ g () x` mein pehlay g evaluate ho ga, phir f, phir f execute ho ga, phir g¹.
- Decorators ko decorator factories bhi banaya ja sakta hai, yani aap aik function likh saktay hain, jo aik decorator return karta hai. Is say aap decorators ko customize kar saktay hain, aur un ko parameters bhi pass kar saktay hain. Masalan, `function log (message:  string) { return function  (target:  any,  propertyKey:  string,  descriptor:  PropertyDescriptor) { console. log (message); }; }` aik decorator factory hai, jo aik message ko log karnay wala decorator return karta hai¹.
- Decorators ko metadata reflection API kay sath bhi istemal kiya ja sakta hai, yani aap aik element kay baray mein metadata bhi define aur access kar saktay hain. Is kay liye aap ko `reflect-metadata` package install karna parta hai, aur `emitDecoratorMetadata` compiler option enable karna parta hai. Masalan, `import \"reflect-metadata\"; @ Reflect. metadata (\"role\",  \"admin\") class User  { } let user = new User (); let role = Reflect. getMetadata (\"role\",  user);` mein User class ko role metadata assign kiya gaya hai, jo baad mein Reflect API say access kiya ja sakta hai¹.


Declaration of Files 

TypeScript kay declaration files kay baray mein complete details yeh hain:

- Declaration files aik khaas qisam kay files hain, jo TypeScript compiler ko JavaScript libraries ya modules kay baray mein type information deti hain. Yeh files sirf compilation step mein istemal hoti hain, aur JavaScript code ko describe karnay ka aik zariya hoti hain. Declaration files C ya C++ kay header files ya Java kay interfaces ki tarah hoti hain¹.
- Declaration files ko `.d.ts` extension kay sath likha jata hai. Masalan, `jquery.d.ts` aik declaration file hai, jo jQuery library kay baray mein type information rakhti hai¹.
- Declaration files ko aik say zyada tareeqon se banaya ja sakta hai. Aap khud say aik declaration file likh saktay hain, ya TypeScript compiler ko `--declaration` option kay sath chala kar aik declaration file generate karwa saktay hain. Aap TypeScript Language Service ko bhi istemal kar saktay hain, jo aap kay code ko analyze kar kay aik declaration file suggest karta hai¹.
- Declaration files ko aik say zyada tareeqon se istemal kiya ja sakta hai. Aap aik declaration file ko aik TypeScript file mein reference tag kay sath include kar saktay hain. Masalan, `/// <reference path=\"jquery.d.ts\" />` aik reference tag hai, jo jquery.d.ts file ko include karta hai¹. Aap aik declaration file ko aik module kay sath import kar saktay hain. Masalan, `import * as $ from \"jquery\";` aik import statement hai, jo jquery module ko import karta hai, aur us ki declaration file ko bhi load karta hai¹. Aap aik declaration file ko aik TypeScript project mein tsconfig.json file kay sath include kar saktay hain. Masalan, `"include": ["./src/**/*", "jquery.d.ts"]` aik include option hai, jo src folder kay tamam files aur jquery.d.ts file ko include karta hai¹.
- Declaration files ko mukhtalif tareeqon se likha ja sakta hai, jo library ya module ki structure kay mutabiq hotay hain. Aap aik global library kay liye aik global declaration file likh saktay hain, jo global variables, functions, ya objects ko declare karta hai. Masalan, `declare var $: JQueryStatic;` aik global declaration hai, jo $ variable ko declare karta hai¹. Aap aik modular library kay liye aik modular declaration file likh saktay hain, jo export statements istemal karta hai. Masalan, `export function ajax(settings: JQueryAjaxSettings): JQueryXHR;` aik modular declaration hai, jo ajax function ko export karta hai¹. Aap aik UMD library kay liye aik UMD declaration file likh saktay hain, jo global aur modular dono tareeqon se istemal ho sakta hai. Masalan, `export as namespace _;` aik UMD declaration hai, jo _ namespace ko export karta hai¹.
