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




