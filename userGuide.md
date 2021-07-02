# Conference Management Tool for ICAF
**This is the user guide for the Conference Management Tool for "International Conference on Application Frameworks" also known as [ICAF](https://icaf-sliit.herokuapp.com/).** 

**To get a more technical idea of the system use our [technical report](reports/technicalReport.pdf ':ignore'). Checkout our [developer guide](devGuide.md) if you're a developer.**
<hr />

# Sign up

A user who has not registered can register as either an attendee, a researcher or a workshop presenter via the sign up form. 

## Attendee

If a user registers as an attendee, a payment should be made up front. This is the attendance fee for the conference.

![](images/signup_attendee.png ':size=700')

## Researcher & Workshop presenter

When a user registers as either a researcher or a workshop presenter, the respective document should be uploaded. For a researcher, this is the research paper. For a workshop presenter, this is the workshop proposal.

![](images/signup_researcher.png ':size=700')

# Sign in

Any user who has previously signed up can sign in to the system using the sign in form. After entering the credentials, if they are validated, users are redirected to the user profile.

![](images/signin.png ':size=700')

# User profile

User accounts differ based on the user role.

## Attendee

If the user is an “Attendee”, the entered contact details can be viewed.

![](images/profile_attendee.png ':size=700')

## Researcher

If the user is a “Researcher”, the entered contact details and the document can be viewed. If needed the document can also be downloaded. The status of the document is also displayed in the user account. The status can be either “pending”, “accepted” or “rejected”.

![](images/profile_researcher_pending.png ':size=700')

If only the status is “accepted”, the researcher can proceed for making the payment for the research paper presentation. After making the payment the status will be displayed as “paid”.

![](images/profile_researcher_accepted.png ':size=700')

## Workshop presenter

If the user is a “Workshop Presenter”, the entered contact details and the document can be viewed. Same as before, If needed the document can also be downloaded and the status of the document is also displayed as either “pending”, “accepted” or “rejected”.

# Downloads

The public pages include a download page, where anyone can download sample research papers, sample workshop proposals, the research paper template and the workshop proposal template.

![](images/download.png ':size=700')