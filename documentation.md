
##How are facilityType added to dataLayer?
let fTypeOptions = document.querySelectorAll('.facilitytype--option')

<!-- line 239 -->
fTypeOptions.forEach((elem) => {
    elem.addEventListener("change", function(event) {
      var item = event.target.value;
      dLInputObject.facilityType = item; 
    });
  });

## How are facilityType added to dataLayer?
// cooling towers or not - start variables
let doesHaveCoolingTowers = true;
// The radio button for having cooling towers or not
let hasCoolingTowersRadioBtn = document.querySelector('#hasCoolingTowers')
let noCoolingTowersRadioBtn = document.querySelector('#noCoolingTowers')

  // When the hasCoolingTowers radio is clicked
  hasCoolingTowersRadioBtn.addEventListener('change', (e) => {
    doesHaveCoolingTowers = true
    dLInputObject.doesHaveCoolingTowers = doesHaveCoolingTowers
  })
  // When the noCoolingTowers radio is clicked
  noCoolingTowersRadioBtn.addEventListener('change', (e) => {
    doesHaveCoolingTowers = false
    dLInputObject.doesHaveCoolingTowers = doesHaveCoolingTowers
  })





self-assessment-simple-success.html
- - - - - - - - - - - - - - - - - -
### On init
window.dataLayer.push({
  'selfAssessmentSubmission': true,
  'whichPage': 'simple-success',
  'which-flow': 'self-assessment-simple-steps'
});

### On submit
window.dataLayer.push({
  'scheduledMeeting': true
});


self-assessment-simple-success.html
- - - - - - - - - - - - - - - - - -
### On init
window.dataLayer.push({
  'selfAssessmentSubmission': true,
  'whichPage': 'simple-success',
  'which-flow': 'self-assessment-simple-steps'
});

### On submit
window.dataLayer.push({
  'scheduledMeeting': true
});
