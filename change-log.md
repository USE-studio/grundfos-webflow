text--blue
<!-- Ex. Don’t know? Contact us here -->

TODO
simple-success
- add header to simple-success
- check up on email and name form data (Full Name 2:)
- Hide second Schedule Meeting button

- undo hasNotChiller on we are sorry slide
- set power to change on cloned inputs
- add white-space nowrap to add chiller button
- if the amount of chillers step remains then pass the number to next step (chillerAmount)
- redirect if noHasCooling to eg. /no-cooling or /we-are-sorry
- Don’t know? Contact us here link mailto
- hide disable functionality of pieprogress if to hard
- max height for form wrapper
- fix the header and repsonsive styling
- put icons in buttons
- change AllLinks decoration
- hide the price in the simple flow
- fix dot navigation for carousel or find another


FIX
- chiller input is not focusable, error if a char is in input

TODO - edge case
- If no is selected and the yes aferwards one should be able to proceed


### Names
#successActionWrapper is the wrapper after the simple flow on success page

## Styles
Schedule Meeting
max-width: 335px

### Style names
smalllabeltext
smalllabeltext--blue

### Rules
max-width SectionInner - 1040px



Section.SectionEmployee
  SectionInner



## Guides

### Where was changes made
 -- webflow = means that change (version) is only Webflow
 -- vscode = means that change (version) is only VS Code

 If it doesn't contain a suffix then it is a mutual iteration

file download on case studies page -- webflow






Loose notes
<div id="formWrapToBeCloned" class="form-wrap extra-space form-wrap-chiller"
  style="transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg); transform-style: preserve-3d; opacity: 1;">
  <label for="Chiller-1-kW" class="field-label">Chiller 1</label>
  <input
    type="number"
    class="text-field-2 w-input"
    maxlength="256"
    name="Chiller-1-kW"
    data-name="Chiller 1 kW"
    placeholder="Input kW"
    has-input-power-to-enable="1"
    id="Chiller-1-kW"
    required=""
  >
</div>
