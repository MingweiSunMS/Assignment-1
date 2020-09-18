# Assignment-1
assignment one for 5100
---------------------------------------------------------------------------
QUESTION #1 Design a course management system

Student:
	data: emailAddress, loginCredentials, name, finishedAssignment
	behavior: login, submitAssignment, delateSubmission, click

courseManagementSystem:
	data: assignment
	Behaviors: sendSubmissionComformation, sendDelateComformation, sendTograder, showGrade, allCourseInstructorAndAssistant

Assignment:
	data: assignmentName
	Behavior:

Grader:
	data: name,
	Behavior: sendGradeToCourseManagementSystem





Student poppy;
courseMamagementSystem canvas;
poppy.login(logimCredemtials);
Assignment hw1 = poppy.click(assignmentName);
poppy.submitAssignment(hw1);
if canvas getSubmittedAssignment:
	canvas.sendToInstructor(poppy.finishedAssignment, poppy.emailAddress);
	canvas.sendSubmissionComformation(poppy.emailAddress);
	if poppy want to make changes:
		poppy.delateSunmission(hw1);
		canvas.sendDeleteComformation(hw1, poppy);
	else
		canvas.sendToGrader(hw1, grader);
		grader Mark = canvas.allCourseInstructorAndAssistant;
		Mark.sentGradeToCouragementSystem
else assignment has no submission
-------------------------------------------------------------------------------------------------------------------
#2 Design a pet adoption platform

customer:
	data: name, loginCredentials, Address, emailAddress, applicationForm
	Behaviors: login, submitApplicaiton, acceptAdoption, requestCancelApplication, search, requestPickup

AdoptionSystem:
	data: puppies, AdoptCenter
	behaviors: sendApplicationComformation, submitApplication, sendToAdoptionCenter, SendPickUpComformation, SendCancelationComformation

Puppy:
	data: brand, size, color
	Behaviors:

Adoptcenter:
	data: applicationReviewer
	Behavior: sendApplicationToReviewer, selectReviewer, sendReminder

applicationReviewer:
	data: name
	Behavior: reviewApplication, sendApproveNotice, sendDeniedNotice, alllocateReviewer





Customer poppy;
AdoptionSystem petsfinder;
Adoptcenter akchome
poppy.login(loginCredentials);
Poppy chihuahua = poppy.search(brand, size, color);
if petsfinder isInStock
	poppy.submitApplicaiton(chihuahua);
	petsfinder.sendApplicationComformation(poppy.emailAddress);
	if poppy change her mind
		poppy.requestCancelApplication(chihuahua);
		petsfinder.sendCancelationComformation(chihuahua);
	else
		petsfinder.sendToaAdoptionCenter(chihuahua, akchome);
		if akchome receive this applicaiton
			akchome.sendApplicationToReviewer;
			applicationReviewer.reviewApplication(chihuahua)
			applicationReviewer mark = akchome.selectReviewer;
			if mark approve the application
				mark.sendApproveNotice("******");
			else mark denied the application
				mark.sendDeniedNotice(00000000);
		else
			akchome.sendReminder(poppy.emailAddress);
else petsfinder outOfStock
			
---------------------------------------------------------------------------------------------

#3 Design an app to book airline ticket.

customer:
	data: name, dob, phone, emailAddress, loginCredentials, creditCard
	Behavior: login, buy, requestCancellation, requestRefund, Search

TravelAgentApp:
	data: flight
	behavior: sendReceipt, checkOut, refund, sendToAirlineCompany

flight:
	Data: time, departure, desternation, class, price
	Behaviors: 

AirlineCompany:
	data: tickets
	behaviors: sendTicketComformation, sendBordingPass, selectAirline, sendDeniedComformation




Customer poppy;
TravelAgentApp priceline;
poppy.login(loginCredentials);
Flight ticket = poppy.search(time, departure, desternation, class, price);
	if priceline isInStock
		poppy.buy(ticket);
		priceline.checkout(poppy.dob, poppy.phone, poppy.emailAdress, poppy.CreditCard);
		priceline.sendReceipt(poppy.emailAdress);
		if poppy change her mind
			poppy.requesCancellation(ticket);
			priceline.refund(ticket, poppy);
		else
			priceline.sendToAirpineCompany(ticket);
			if airlinecCompany get the customer infomation
				airlineCompany.sendTicketComformation(ticket, poppy);
			else airlineCompant not get the customer infomation
				airlineCompant.sendDeniedComformation(ticket, poppy);
	else ticket outOfStock


-------------------------------------------------------------------------------------------------------------------
#4 Design a course registration platform.


customers:
	data: emailAddress, name, loginCredential, studentId
	behavior: login, search, requestEnrollcourse, requestDropCourse

CourseResteration Website:
	data: courses
	behaviors: sendEnrolledComformation, sendDroppedComformation, registerCourse, sendWaitlistComformation, sendToInstructor

Course:
	data: name, time, crnNumer
	behaviors:




customer poppy;
courseResteration Website banner;
poppy.login(loginCredentials);
Course cse174 = poppy.search(name, time,crnNumber);
if cse174 have empty seat
	poppy.requestEnrollCourse(sce174);
	banner.registerCourse(poppy.studentId, cse174);
	banner.sendEnrolledComformation;
	if poppy want to drop the course
		poppy.requestDropCourse(poppy.emaillAddress, cse174);
		banner.sendDroppedComformation(poppy.emaillAddress, cse174);
	else banner.sendToInstroctor
else cse not have emoty seat
	banner.sendWaitlistComformation(poppy.email, cse174);
  
---------------------------------------------------------------------------------------------------------------------------------------

#5 Order food in a food delivery app

Customer:
	Data: phoneNumber, name, address, loginCredentials, pay, creditCard
	behaviors: Login, setOrder,tracking, requestCancelOrder, requestRefund, writeReview, search, pay

DeliveryApp:
	Data: Resturants, orderInfo, checkOut
	Behaviors: sendReceipt, CheckOut, refund, sendToDeliveryPerson, alllocateCourier

Resturant:
	Data: entrees, Price, Size
	Behaviors: sendcComformation

OrderInfo:
	Data:entrees, size
	Behavior:


DeliveryPerson:
	Data: Name, TranspotationInfo
	Behaviors: DeliveryFood; ContactCustomer





Customer poppy;
DeliveryApp ubereat;
popppy.login(loginCredentials);
Resturants popeyes = poppy.search(entrees, size, price);
OrderInfo kidsmeal = poppy.setOrder(entree, size);
if ubereat getOrderInfo
	poppy.pay(kidsmeal);
	ubereat.checkout(poppy.address, poppy.creditCard, poppy.phoneNumber)
	resturant. sendacaomformation(kidsmeal);
	ubereat.sendReceipt(poppy, phoneNumber);
  if poppy change her mind
		poppy.requestCancelOrder(popeyes);
		ubereat.refund(popeyes, poppy);
	else
		ubereat.sendToDeliveryPerson(poppy.phoneNumber, poppy.address);
		deliveryperson mark = deliveryPerson.alllocateDeliveryPerson;
		mark.contactCustomer(poppy);
		mark.deliveryFood(popeyes, poppy.address);
		if poppy satisfied with the food
			poppy.wroteReview("*********");
		else
			poppy.writeReview("000000000");
			poppy.requestRefund(popeyes, ubereat);
			ubereat.refund(poppy);
else ubereat doNotGetOrderInfo

	




