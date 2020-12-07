# Export-Named-Exports

Named exports are also distinct in that they can be exported as soon as they are declared, by placing the keyword export in front of variable declarations.

In menu.js

export let specialty = '';
export function isVegetarian() {
}; 
function isLowSodium() {
}; 
The export keyword allows us to export objects upon declaration, as shown in export let specialty and export function isVegetarian() {}.
We no longer need an export statement at the bottom of our file, since this behavior is handled above.


### QQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQ


1.
Let’s add some additional data to our airplane.js file.

Continue by adding more data to objects within the availableAirplanes variable.

To the first object AeroJet, add a property maxSpeed with a value of 1200 and a property minSpeed with a value of 300.

To the second object SkyJet, add a property maxSpeed with a value of 800 and a property minSpeed with a value of 200.


Hint
let availableAirplanes = [
{name: 'AeroJet',
 fuelCapacity: 800,
 availableStaff: ['pilots', 'flightAttendants', 'engineers', 'medicalAssistance', 'sensorOperators'],
 maxSpeed: 1200,
 minSpeed: 300
}, 
{name: 'SkyJet',
 fuelCapacity: 500,
 availableStaff: ['pilots', 'flightAttendants'],
 maxSpeed: 800,
 minSpeed: 200
}
];
2.
Within the flightRequirements object, add a property requiredSpeedRange and set this equal to 700.


Hint
let flightRequirements = {
  requiredStaff: 4,
  requiredSpeedRange: 700
};
3.
Continuing with the same file, add a new function meetsSpeedRangeRequirements() that takes three arguments maxSpeed, minSpeed and requiredSpeedRange.


Hint
function meetsSpeedRangeRequirements(maxSpeed, minSpeed, requiredSpeedRange) {
};
 
4.
Within the meetsSpeedRangeRequirements function, create a variable range, and set it to the difference between maxSpeed and minSpeed.


Hint
function meetsSpeedRangeRequirements(maxSpeed, minSpeed, requiredSpeedRange) {
  let range = maxSpeed - minSpeed;
};
5.
In the body of the meetsSpeedRangeRequirements() function, create logic to check if the range is greater than the requiredSpeedRange.

The function should contain this logic:

if the `range` is greater than the `requiredSpeedRange`
  return true
else 
  return false 

Hint
function meetsSpeedRangeRequirements(maxSpeed, minSpeed, requiredSpeedRange) {
  let range = maxSpeed - minSpeed;
  if (range > requiredSpeedRange) {
    return true;
    } else {
    return false;
  }
};
6.
Use export to export the variables as soon as they are declared, and remove the export statement at the bottom of the file.


Hint
export let availableAirplanes = [...];
 
export let flightRequirements = {...};
 
export function meetsStaffRequirements(){
...
};
 
export function meetsSpeedRangeRequirements(){
...
};
