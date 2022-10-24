# Exploratory Testing Charter
> Simple example for an online shopping cart

# 1. Purpose of this document      

This document aims at defining the main aspects in guiding the exploratory testing activity of an online shopping cart for which no system specifications or test scripts exist. Having a defined testing activity scope will help in measuring achievements effectively and finishing the exploratory testing activity in a timeboxed fashion. 

# 2. System Under Test
The SUT will be an online shopping cart called OpenCart made available for practicing testing. This shopping cart offers many features that can be tested through multiple scenarios. 

**Test Environment:**
- URL:  http://opencart.abstracta.us/

**Browser platform & version:**
- Google Chrome 106.
- Microsoft Edge 106.
- Mobile Android (version to be defined according to the tester device). 


# 3. Intended goals from testing  
- Exploring the online shopping cart application by executing a few core scenarios from an end-user (a buyer) perspective (ex: searching and purchasing a product..). 
- Identifying usability issues in the product purchase flow. 
- Exploring different scenarios for price calculation and identifying potential defects in this specific area. 
- Exploring the behavior of the shopping cart on a mobile device by following the same core scenarios executed on the web version. 


# 4. Features to cover during the testing
- [ ] Product search. 
- [ ] Product info.
- [ ] Shopping cart.
- [ ] Checkout process.
- [ ] Order status, cancel and return.
- [ ] Creating and managing my account info.


# 5. Tests types to cover
Following are the differents test types that need to be covered throughout the exploratory testing activities:

- **Functional testing**: evaluating the functional quality characteristics of the system, such as completeness, correctness, and appropriateness. The system functions that need to be covered are listed in section 4.

- **Usability testing:** since it's a broad topic and testers can be easily lost when doing usability testing, we recommend to use the following techniques to determine to which extent the SUT is easy to operate and attractive to the users: 

   *“Experience-based” technique: observations can be given by the tester according to his experience and knowledge, in such a case, the tester needs to clearly explain his observation and why improvement is recommended in a specific area or flow. Referring to trusted UX sources is also a valid option.

   *“Hallway” technique:  in this case, the main tester would play the role of a facilitator of a few testing sessions by selecting a few random people who are given access to the online shopping cart to complete some scenarios. During scenarios execution, the tester will record observations and log issues users faced in terms of usability. 


# 6. Testing strategy to follow
We will be following a combination of the following test strategies identified according to the nature of the system under test and the testing context: 

- *“Reactive”* strategy: since this is about exploratory testing, testing will be reactive to the system being tested, and the events occurring during test execution, rather than being pre-planned. Tests will be designed and implemented, and will immediately be executed in response to knowledge gained from prior test results.

- *“Risk-based”* strategy: since we’re dealing with product purchases, online payments and end users personal info, it’s highly recommended to identify some critical vulnerability. Since security is a broad topic, following are few ideas that the tester can star with: 
   -  Verifying security aspects related to the technical implementation and framework used (in this case PHP) from knowledgeable and trustworthy organizations.
   - Using open source tools to conduct in-depth security audits (Cross Site Request Forgery, SQL injection…).  
   - Verifying that the system doesn’t allow access to critical functionalities in case of logged out users such as the checkout process. 
   - …
   - 
# 7. Tests output

- **Test notes:** Step by step “journal” of the exploratory tests. The format for this is a sentence describing what actions were taken when testing, followed by bullets to describe the observations and steps performed to complete the action described.

- **Bugs:** what bugs were found during the exploratory test. The format is a sentence bug name, followed by a section titled: “Steps to Reproduce,” then bulleted steps, a “Expected Results:” section then an “Actual Results” section. Each bug should be numbered.

:arrow_right: We invite you to use dedicated [GitHub Issues templates](https://github.com/mohammed-ibenayad/exploratory_testing_opencart/issues/new/choose) to log your bugs and test notes

