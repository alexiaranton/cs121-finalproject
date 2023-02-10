
Sawa is a a new programming langauge founded in Python

<h1>Sawa: A Bisaya Programming Language</h2>

## Geting Started


### Prerequisites

You need llvmlite and sly modules to run the project.
* llvmlite
  ```sh
  pip install llvmlite
  ```

* sly
  ```sh
  pip install sly
  ```

## Usage

### Compiling the code

Extention for Sawa is .sa , to compile .sa files use
```sh
python run.py <filename.sa>
```

This will generate a .ll intermediate code file in the same folder where code is present and output the result too.


### Documentation:

#### General

<code>sabot</code> is used to define a function. One must define <code>main</code> function in the project. Example :
```sh
sabot int main() {
    # code goes here
    sugod balik 0     #similar to return
}
```

<code>sugod</code> is used to initialize any statement.

#### Print

<code>sugod patik(<strings here>)</code> is used to print the strings :
```sh
sabot int main() {

    sugod patik("Bidyohi ko! Agoy!")
    sugod patik("Bidyohi ko, mapriso ka!) #this is comment

    sugod balik 0
}
```
  
#### Defining Variables

```sh
sabot int main() {

    sugod x=5
    sugod y=9.0
    
    sugod balik 0
}
```

#### Conditional Statements

```sh
sabot int main() {

    sugod num1 = 18
    sugod rem = num1 % 2
    sugod kung rem == 0{
        sugod patik('Even')
    } 
    imbis{
        sugod patik('Odd')
    }

    sugod balik 0
}

```
  
#### Iterations

```sh
sabot int main(){
    sugod i = 0
    samtang i < 10
    {
        sugod patik('Hello ')
        sugod i = i+1
    }
   sugod balik 0
}

```
                 
#### Calling Functions

```sh
sabot int hello() {
    sugod patik("Agoy! \n")
    sugod balik 0
}

sabot int main(){
    hello()
    sugod patik("Mapriso ka!")
    sugod balik 0
}

```



