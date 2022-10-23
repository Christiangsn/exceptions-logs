# <h1 align="center"> @DECORATORS-TS/EXCEPTION-LOGS </h1>
### version: 0.0.3-beta.1

# :bookmark_tabs: About the Project
Based on design patterns decorators, this functionality will allow you to implement an exception log decorator that brings you custom information...

# :pushpin: How to install and run the project

### Install

```bash
yarn add -D @decorators-ts/exceptions-logs
```
or

```bash
npm install -D @decorators-ts/exceptions-logs
```

### :question: How does this help me?

As seen in the images above, the decorator implements custom logs, thus, sending you the controller execution time and also the error reason, if it happens

### How to use?

```bash
 import { Execpetion } from '@decorators-ts/exceptions-logs'
```

on the top line of your class function, invoke the method


```bash
  @Execpetion({
      methodName: 'DevelopmentController',
  })
```
###  parameters
  - methodName: (String) - Name of the class or function to be executed
  - execeptionError: (Error | any) - By default it will return a new Error('Internal Server Error'), but if you want to customize the return in case of an error, make the notation in this parameter

###  return
  - the event tasks will be displayed in your console, thus delivering customized information in case of error or success

# EXAMPLE
![Screenshot](exemp.png)

my console in execution success
![Screenshot](success.png)

my console in execution fails
![Screenshot](error.png)
