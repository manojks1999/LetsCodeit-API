# LetsCodeit

### Introduction to LetsCodeit API
It supports multiple langauge all of is free.

### Executing and fetching Output.
Use a POST request with specified fileds to get a Output.

### List of supporting languages:
Make a GET request to 
> https://letscodeit-api.herokuapp.com/list

Request:

> GET : https://letscodeit-api.herokuapp.com/list

Response:
```
[
    {
        "language": "java",
        "compilerVersion": "11.0.15"
    },
    {
        "language": "cpp",
        "compilerVersion": "11.2.0"
    },
    {
        "language": "py",
        "compilerVersion": "3.7.7"
    },
    {
        "language": "c",
        "compilerVersion": "11.2.0"
    },
    {
        "language": "js",
        "compilerVersion": "16.13.2"
    },
    {
        "language": "go",
        "compilerVersion": "1.18.3"
    },
    {
        "language": "cs",
        "compilerVersion": "6.12.0.140"
    }
]
```

Endpoint to execute Codes:
> https://letscodeit-api.herokuapp.com/

### Fields:
#### Input Parameters:

- code:
- language:
- input:

#### Output Fields:

- success
- timestamp
- output
- language
- version

### Sample:

#### Request

```
code:
#include <iostream>
int main() {
    std::cout << "Hello World!";
    return 0;
}

language:
cpp

input:
```

#### Response:
```
{
    "success": true,
    "timestamp": "2022-07-12T03:09:05.667Z",
    "output": "Hello World!",
    "language": "cpp",
    "version": "11.2.0"
}
```
