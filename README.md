# birthdate-calendar
birthdate calendar for angular material using momentjs. <br>
This directive has the neccesary elements for a birthdate picker, a simple input for year that allows 100 as max age, a grid with the months,and a calendarday grid for days. <br>

The only that requires to work fine this directive is adding a $on event on your controller.

### The markup

```<birthdate-calendar  birthdate="user.birthDate"> </birthdate-calendar>```


```js
$scope.$on('updateDate',function(event,data){
  //handle the data as you need 
  $scope.user.birthDate = moment(data).format('YYYY-MM-DD');
})
```
![myimage-alt-tag](https://s24.postimg.org/ye92q04mt/687474703a2f2f7331382e706f7374696d672e6f72672f66.png)
