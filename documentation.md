# dataLayer pushes


## landingpage - start

### Init - start
window.dataLayer.push({
  'event': 'gtm.load',
  'whichPage': 'success',
  'which-flow': 'self-assessment-simple-steps',
  'meetingScheduled': 'true'
});
### Init - end

### which calc button - start
window.dataLayer.push({
  'event': 'gtm.load',
  'whichCalcSavingsBtn': id
});
### which calc button - end

### downloadCaseStudiesBtnWasclicked - start
window.dataLayer.push({
  'event': 'gtm.load',
  'clickedDownloadCaseStudiesBtn': 'true'
});
### onDownloadCaseStudies - end

## succlandingpageess - end





## self-assessment-simple - start

### Init - start
window.dataLayer.push({
  'event': 'gtm.load',
  'stepValue': stepValue,
  'whichPage': 'self-assessment-simple-steps',
  'whichFlow': 'self-assessment-simple-steps'
});
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


### Lastly - start 
<!-- if stepValue === 5 and if progress button is clicked -->
window.dataLayer.push({
  'event': 'gtm.load',
  'stepValue': '6',
  'submission': dLInputObject
});
### Lastly - end 

### Other
forwardLinkcopiedToClipboard: "true"

## self-assessment-simple - end




## calculation - start
window.dataLayer.push({
  whichPage: "self-assessment-calculation",
  which-flow: "self-assessment-simple-steps",
  calculationWasMade: "true"
})
## calculation - end




## success - start

### Init - start
window.dataLayer.push({
  'event': 'gtm.load',
  'whichPage': 'success',
  'which-flow': 'self-assessment-simple-steps',
  'meetingScheduled': 'true'
});
### Init - end

### downloadCaseStudiesBtnWasclicked - start
window.dataLayer.push({
  'event': 'gtm.load',
  'downloadCaseStudiesBtnWasclicked': 'true'
});
### onDownloadCaseStudies - end

## success - end











## self-assessment-simple-newsletter - start

### Init - start
window.dataLayer.push({
  'event': 'gtm.load',
  'stepValue': 'noCoolingTowers',
  'whichPage': 'self-assessment-simple-newsletter'
});
### Init - end

## self-assessment-simple-newsletter - end




## newsletter-subscription-success - start

### Init - start
window.dataLayer.push({
  'event': 'gtm.load',
  'whichPage': 'newsletter-subscription-success',
  'subscribedToNewsletter': 'true'
});
### Init - end

## newsletter-subscription-success - end












## Old
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



<!--  --> = missing (Needs implementation)

self-assessment-simple-steps.html
- - - - - - - - - - - - - - - - - -
### On init
window.dataLayer.push({
  <!-- 'whichPage': 'self-assessment-simple-steps', -->
  'which-flow': 'self-assessment-simple-steps'
});

### On submit
window.dataLayer.push({
  'scheduledMeeting': true
});
- - - - - - - - - - - - - - - - - -



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
- - - - - - - - - - - - - - - - - -




self-assessment-simple-help.html
- - - - - - - - - - - - - - - - - -
### On init
 window.dataLayer.push({
  'whichPage': 'self-assessment-simple-help',
  'askedForHelp': true
});

### On submit
No submit
- - - - - - - - - - - - - - - - - -