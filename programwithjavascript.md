function welcomeHere(){
  var today= new Date(); 
  var hourNow = today.getHours(); 
  var greeting; 
  if (hourNow > 18) { 
  greeting= 'Take a whiff with one of our imported candles and feel like your else where'; 
  }
  else if (hourNow > 12) { 
  greeting = 'Where do you wanna go to nasally today?'; 
  }
  else if (hourNow >= 0) { 
  greeting = 'In the early morning, light an amazing scent to start the new day!'; 
  }
  else { 
  greeting = 'Welcome!'; 
  }
  return '<h3>' + greeting + '</h3>' ;   
  }
function addUserName(){
  var name = prompt ("What is your name?")
  var greeting
  if (name !==""){
      greeting = "hello" + name
  } 
  return '<h3>' + message + '</h3>';
}
