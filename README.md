# birthdate-calendar
birthdate calendar for angular material using momentjs. <br>
This directive has the neccesary elements for a birthdate picker, a simple input for year that allows 100 as max age, a grid with the months,and a calendarday grid for days. <br>

The only that requires to work fine this directive is adding a $on event on your controller.

```js
$scope.$on('updateDate',function(event,data){
  //handle the data as you need 
  $scope.user.birthDate = moment(data).format('YYYY-MM-DD');
})
```
![myimage-alt-tag](http://s18.postimg.org/f1vbd36vt/birthdate_Preview.png)
