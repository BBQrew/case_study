# Project

## 1 create model class "Job"

> php artisan make:model Job -mcr

```-mcr```

- ```--migration``` Create a new migration file for the model
- ```--controller``` Create a new controller for the model
- ```--resource``` Indicates if the generated controller should be a resource controller

## 2 create policy class "JobPolicy" for model class "Job"

> php artisan make:policy JobPolicy -model:Job

doesn't work

response:
> Too many arguments to "make:policy" command, expected arguments "name".

### 2.1 use instead

> php artisan make:policy JobPolicy -m=Job

does the job
