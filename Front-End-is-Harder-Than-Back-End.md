# Front End is Harder Than Back End

Posit: common belief that back end development is `harder` than front end development likely is false.  It's very likely false in practice, maybe perhaps also likely in theory.

### Modern Web & Mobile Application Development is Hard

Common belief is back-end work is proper engineering, while front-end work is practically art class.

In practice this is (likely) the exact opposite. 

### Text is Binary, UI/UX is Dynamic

* Back end => data and architecture as text
* Front end => data and architecture as user interface

* Back-end => client is the customer.  A machine (the client, aka front-end) is user. 
* Front-end => human is the customer.  A live person is the user.

### Unwanted Feedback 

Another way to consider this problem: because everyone can consume an app (client), and mostly clients consume back-ends, the feedback is VERY different.  

Front-end feedback is rich and diverse.  Back end feedback is often binary.  Most of this feedback is worthless, but nevertheless people are very often quick to provide commentary on layout, text content and pixel location. 

In contrast, back end development is very binary.  Is the text right or wrong?  HTTP 200 or 404? (The other codes are meaningful too, I'm having some fun! ;) )   

If the data is correct, you may pass.  Format the data once, send/receive forever.  

### Does Data got style? 

Well it has a model.  But most front-ends consume REST endpoints that spew out blobs.   

Blobs of data more often than not contain fields that are useless/redundant.  Some `.then()` block will mutate the data into the form you want, but you're judged primarily on whether or not the data can be sent over a wire.

Front end style can be, and more often than not, IS ENDLESSLY DEBATED by anyone with eye balls.  Functionality is eschewed for presentation.  There is little science, and much emotion in the process of UI/UX, making the human-problems associated with front-end web development far more time-consuming and challenging than back-end. 

### Runtime Environments 

Back end runtime is some machine on the cloud.  This can be complex, but most applications are not facebook, and don't require sophisticated Docker config and server mgmt.  Bundle it up and slam it on a virtual machine, which will run that code in a predictable environment every time.  Code runs in the same environment every time, produces the same structured result / API.

On the front end it seems everything is always different, as far as runtime goes. The code executes in millions of unique environments and devices.  Thousands of phones and screen sizes.  Disparate browser-specific specs, it's more likely than not the environment your app is running is unique! What a nightmare. 

### Features 

Back end features are more easily distilled and concrete.  Front end features are vague and amorphous.  This related to the feedback portion, but is also standalone issue. 

Features on the front end contain much hand-waving and assumptions.  Because product managers might not be aware of the Box Model, or basic UX principals (but rather is advocating for an arbitary feature-set on behalf of the paying customers).  Predicting cross-site behaviour of changes on client-side code can be very tricky. 

### Javascript

There are good parts, and bad parts.  But there are no alternatives.  Browsers run JS, and front-end work is done in JS.

Back end work is more flexible and thus plug-and-play-like.  Consume and produce text, whatever does this, doesn't matter.  JS, GO, Python, Ruby, Elixor, whatever.  Just send and receive text reliably and quickly , KTHNX.

### Future Considerations? 

AI... design is going win the labout market over data architects and network specialists. Maybe it already has (Jobs vs Woz?).

### FLAWS 

Hell yes.  There are lots.  I typed this up quickly, devs please chime in and correct the errors above to @Royal_Arse on twitter. 

