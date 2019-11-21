---
lang: en
layout: article_with_sidebar
updated_at: '2018-09-07 13:34 +0400'
identifier: ref_5EkhZ4uD
title: Customer Satisfaction
order: 72
published: true
---
The addon [Customer Satisfaction](https://market.x-cart.com/addons/customer-satisfaction.html "Customer Satisfaction") enables the store admin to follow up with the customers who have made a purchase at the store and collect reviews from them to find out how they rate the store as a whole and the store customer service in particular. 

{% toc %}

## Customer Satisfaction Addon Installation and Setup

To install the addon, follow the guidelines from {% link "Installing Addons from the X-Cart App Store" ref_Vn1mMUw9 %}.
![customer_satisfaction_addon.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/customer_satisfaction_addon.png)

Once the addon has been installed, open the addon settings page to adjust the addon configuration. You can use either the **Go to addon settings page** button on the screen you see when the addon installation has been completed or the **Settings** button in the addon details pop-up in the **My Addons** section:

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![540-go-addon-settings.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/540-go-addon-settings.png)</div>
  <div class="column" markdown="span">![540-settings-button.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/540-settings-button.png)</div>
</div>


The Customer Satisfaction addon settings page is divided into 2 subsections:
1. **General options** - where you can set up the general addon behaviour:
   ![540-settings-page-1.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/540-settings-page-1.png)
   * **Action to send email** : An email with a request for feedback will be sent automatically by the system when an order receives a defined payment or shipping status. Choose between _by payment status_ and _by shipping status_. 
   * **Choose payment/shipping status triggering feedback request** : The name of the setting will depend on the trigger you've chosen for the **Action to send email** setting. Select either payment or shipping status that will imply sending an email with a feedback request.
   * **Delay in days** : Define the time period in days the request for feedback should be delayed for. If you want the survey to be emailed the same day the order obtained the specified payment or shipping status set the setting value to 0 (zero).
   * **Excellent/no-questions-asked rating** : Specify the rating (from 1 to 5, where 5 is an excellent rate) that should not be followed by a survey.
   * **Facebook fanpage URL** : Specify your store Facebook fanpage URL if applicable.
2. **Feedback survey top text** - where you can define the text welcoming a customer to answer a feedback survey:
   ![540-settings-page-2.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/540-settings-page-2.png)
   Decide whether you need to change the landing page text suggested by default for "Auful/Bad/Fair/Good/Excellent" rates. This text welcomes customers on a post-feedback survey page.
   ![landing-page-text.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/landing-page-text.png)

Once the basic addon setup has been completed, proceed to the **Feedback questions** section (**Orders** -> **Feedback questions**) to configure the questions that will be presented to a customer as a follow-up survey.
![540-feedback-questions.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/540-feedback-questions.png)

Here you can reorder the existing questions by drag-n-dropping them or delete them completely. Also you can add new questions if necessary. Use the **New question** button for the purpose:

![new-question.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/new-question.png)

Don't forget to **save changes** when you are done.

## Customer Experience

When an order gets a status as defined in **Choose payment status triggering feedback request** a customer receives an email with a suggestion to rate the order experience:

![fedback-email.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/fedback-email.png)

Clicking on a rate forwards the customer to a store page where he can answer the survey questions as they are configured in the **Feedback questions** section to clarify his position and leave comments.

![cus-good.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/cus-good.png)

## Admin Experience

All customers' feedbacks are registered in the **Customer feedback** section in the store admin area (**Orders** -> **Customer feedback**):

![customer-feedback.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/customer-feedback.png)

To manage a feedback click the **[...]** button opposite the feedback in question. You'll be redirected to the **Manage Customer Feedback page** where you can check for the survey details and the comments provided by the customer. 

![manage-feedback.png]({{site.baseurl}}/attachments/ref_5EkhZ4uD/manage-feedback.png)

Each feedback except for the 'excellent' ones get the NEW status that you can change to 'IN PROGRESS' or 'CLOSED' when the feedback is addressed. The 'excellent' feedbacks get the CLOSED status automatically. 

To process the feedback further you can contact the customer by email to thank him for the feedback left or to help in case of any questions.
