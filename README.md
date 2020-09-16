# Assignment-1
assignment one for 5100
----------------------------------------------------------------------------------------------------------------------------------------------------
#1--Food Delivery App
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

-------------------------------------------------------------------------------------------------------------------------------
#2 pet adoption system

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
			akchome.sendReminder
else petsfinder outOfStock
			
-----------------------------------------------------------------------------------------------------------	
#3 Course Management
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

---------------------------------------------------------------------------------------------------------------------------------------





