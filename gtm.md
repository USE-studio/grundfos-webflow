# dataLayer pushes


## self-assessment-simple - start

### Init - start
'stepValue': stepValue,
'whichPage': 'self-assessment-simple-steps',
'whichFlow': 'self-assessment-simple-steps'
### Init - end


### Continuous - start
<!-- Move forward -->
window.dataLayer.push({
  // 'event': `current stepValue is: ${stepValue}`,
  'event': 'gtm.load',
  'stepValue': stepValue
});

<!-- Move backward -->
window.dataLayer.push({
  // 'event': `current stepValue is: ${stepValue}`,
  'event': 'gtm.load',
  'stepValue': stepValue
});
### Continuous - end


### Once - start 
<!-- if stepValue === 5 and if progress button is clicked -->
window.dataLayer.push({
  'event': 'gtm.load',
  'success': true,
  'submission': dLInputObject
});
### Once - end 

## self-assessment-simple - end