---
layout: apply
hidden: true
title: 'Apply to work with us'
description: 'Use the form on this page to apply for a job at St George’s. We cannot be held responsible for any loss of data so we strongly encourage you to write out all longer answers in a text editor and copy them into the form when complete.'
date: 2018-05-09 15:50:54 +0000
---
<form novalidate="" action="https://form.letsdance.agency/ZbM5mMyr" method="POST" class="tab-wrap" data-tabs="3" data-redirect="/thankyou" data-failure="<h3>Error</h3><p>Your application was not sent. Please try again and contact us if the problem persists.</p>" data-loading="<strong>Please wait.</strong> Sending your application." data-success="<h3>Thank you</h3><p>Your application has been submitted.</p>">
    <input type="radio" name="tabs" value="tab-about" id="tab-about">
    <label for="tab-about">1. About you</label>
    <div class="tab-content">
      {% assign jobs = site.jobs | map: 'title' | join: "," %}
      {% include fields/select.html label="Job title" help="Select the job you’re applying for." name="_subject" values=jobs required="true"%}

      <fieldset>
        <legend>Your name and contact details</legend>
        {% include fields/input.html fieldset="contact_details" type="text" name="name" placeholder="Enter your full name" required="true" %}
        <div class="field-group">
          {% include fields/input.html fieldset="contact_details" type="email" name="email" placeholder="Enter your email address" required="true" class="half" %}
          {% include fields/input.html fieldset="contact_details" type="text" name="phone" placeholder="Enter your phone number" required="true" class="half" %}
        </div>

        {% include fields/textarea.html fieldset="contact_details" name="address" placeholder="Please provide your address including postcode" required="true" %}

      </fieldset>

      <fieldset>
        <legend>Diversity</legend>
        <p class="fieldset-intro">Answering the questions below allows us to monitor our commitment to being an equal opportunities employer.</p>
        <div class="alert">The details given in this section are confidential and <strong>will not be considered in any way during the appointment process</strong>.</div>

        {% include fields/radio.html fieldset="diversity" name="age_group" values="16-24,25-34,35-49,50+" %}
        {% include fields/select.html fieldset="diversity" name="ethnicity" values="White  –  English / Welsh / Scottish / Northern Irish / British,White  –  Irish,White - Gypsy or Irish Traveller,White - Other,,Mixed / Multiple - White and Black Caribbean,Mixed / Multiple - White and Black African,Mixed / Multiple - White and Asian,Mixed / Multiple - Other,,Asian  –  Indian,Asian  –  Pakistani,Asian  –  Bangladeshi,Asian  –  Chinese,Asian  –  Any other Asian background,,Black  –  African,Black  –  Caribbean,Black  –  Other,,Other  –  Arab,Other  –  Any other group" %}
        {% include fields/radio.html fieldset="diversity" name="gender" values="Male,Female,Non-binary" %}

        {% include fields/textarea.html fieldset="diversity" name="interview_requirements" help="If you are successful in being invited for an interview do you have any specific requirements, i.e. an interview on the ground floor, information provided large print etc.? If so, please provide details." %}

      </fieldset>

      <fieldset>
        <legend>Convictions</legend>
        <p class="fieldset-intro">This post is exempt from the provisions of section 4 (2) of the Rehabilitation of Offenders Act 1974, by virtue of the Rehabilitation Act 1974 (Exceptions) Order 1975.  Due to the nature of the position, the person appointed would have to be cleared for Child Protection purposes in line with Working Together to Safeguarding (2013). This will include an enhanced Disclosure and Barring Service check (DBS).</p>
        {% include fields/radio.html fieldset="convictions" name="have_you_ever_been_convicted_of_an_offence?" label="Have you ever been convicted of an offence?" values="yes,no" required="true" %}
        {% include fields/textarea.html fieldset="convictions" name="details_of_any_convictions" %}

      </fieldset>

    <div class="tab-footer-navigation">
      <button disabled class="back white">Previous</button>
      <a data-tab="experience" href="#" class="button white">Next</a>
    </div>


    </div>
    <input type="radio" name="tabs" value="tab-experience" id="tab-experience">
    <label for="tab-experience">2. Your experience</label>

    <div class="tab-content">
      <fieldset>
        <legend>Describe your suitability for the role</legend>
        <p class="fieldset-intro">Tell us what experience, skills and abilities you can bring to the job. Match your skills to the person specification, and include skills gained from paid or voluntary work, or through family and leisure activities.</p>
        {% include fields/textarea.html fieldset="suitability" name="information_to_support_your_application" rows="15" maxlength="3000" required="true" %}
      </fieldset>

      <fieldset>
        <legend>Present or most recent employment</legend>
        <div class="field-group">
          {% include fields/input.html fieldset="employment" type="text" name="job_title" class="half"%}
          {% include fields/input.html fieldset="employment" type="text" name="employer" class="half" %}
        </div>
        <div class="field-group">
          {% include fields/input.html fieldset="employment" type="date" name="date_appointed" class="half" %}
          {% include fields/input.html fieldset="employment" type="date" name="date_left" help="Only if you’ve already left this role" class="half" %}
        </div>
        <div class="field-group">
          {% include fields/input.html fieldset="employment" type="text" name="salary_or_hourly_wage" class="half" %}
          {% include fields/input.html fieldset="employment" type="text" name="notice_period" class="half" %}
        </div>

        {% include fields/textarea.html fieldset="employment" name="duties" placeholder="Summarise your main duties and responsibilities" %}
        {% include fields/textarea.html fieldset="employment" name="reason_for_leaving" placeholder="Please state your reason for leaving, if relevant." %}
      </fieldset>

      <fieldset>
        <legend>Previous employment</legend>
        <p class="fieldset-intro">Please provide details of your previous employment.</p>

        <div class="duplicator">
          {% include fields/textarea.html fieldset="previous_employment[$$$]" disabled="true" name="title" %}
          {% include fields/textarea.html fieldset="previous_employment[$$$]" disabled="true" name="employer" %}
          {% include fields/textarea.html fieldset="previous_employment[$$$]" disabled="true" name="dates" %}
          {% include fields/textarea.html fieldset="previous_employment[$$$]" disabled="true" name="reason_you_left" %}
        </div>
      </fieldset>

      <fieldset>
        <legend>References</legend>
        <p class="fieldset-intro">Please provide two references, one of whom must be your present or most recent employer. At least one must be available for us to contact prior to interview.</p>
          <div class="alert">Please ensure you have permission to use these people as referees</div>
        <h3>First referee</h3>
        <div class="field-group">
          {% include fields/input.html fieldset="referee[1]" type="text" name="name" class="half" %}
          {% include fields/input.html fieldset="referee[1]" type="text" name="job_title" class="half" %}
        </div>
        <div class="field-group">
          {% include fields/input.html fieldset="referee[1]" type="text" name="contact_phone" class="half" %}
          {% include fields/input.html fieldset="referee[1]" type="email" name="contact_email" class="half" %}
        </div>
        <h3>Second referee</h3>
        <div class="field-group">
          {% include fields/input.html fieldset="referee[2]" type="text" name="name" class="half" %}
          {% include fields/input.html fieldset="referee[2]" type="text" name="job_title" class="half" %}
        </div>
        <div class="field-group">
          {% include fields/input.html fieldset="referee[2]" type="text" name="contact_phone" class="half" %}
          {% include fields/input.html fieldset="referee[2]" type="email" name="contact_email" class="half" %}
        </div>
      </fieldset>

      <fieldset>
        <legend>Education</legend>
        <p class="fieldset-intro">Please provide details of your formal education, including any schools, colleges and universities attended. Training or short courses should not be listed here; include them in the next section.</p>

        <div class="duplicator">
          {% include fields/textarea.html fieldset="education[$$$]" disabled="true" name="institution" %}
          {% include fields/textarea.html fieldset="education[$$$]" disabled="true" name="qualification" %}
          {% include fields/textarea.html fieldset="education[$$$]" disabled="true" name="grade" %}
          {% include fields/textarea.html fieldset="education[$$$]" disabled="true" name="date" %}
        </div>
      </fieldset>

      <fieldset>
        <legend>Training and short courses</legend>
        <p class="fieldset-intro">Include any additional training you think is relevant to the role here.</p>

        <div class="duplicator">
          {% include fields/textarea.html fieldset="training[$$$]" row="2" disabled="true" name="provider" %}
          {% include fields/textarea.html fieldset="training[$$$]" row="2" disabled="true" name="course_title" %}
          {% include fields/textarea.html fieldset="training[$$$]" row="2" disabled="true" name="grade" %}
          {% include fields/textarea.html fieldset="training[$$$]" row="2" disabled="true" name="date" %}
        </div>
      </fieldset>

      <div class="tab-footer-navigation">
        <a data-tab="about" class="button white back">Previous</a>
        <a data-tab="submit" href="#" class="button white">Next</a>
      </div>

    </div>
    <input type="radio" name="tabs" value="tab-submit" id="tab-submit">
    <label for="tab-submit">3. Submit</label>
    <div class="tab-content">

      <div class="pullout">
        <h3>Equal opportunities</h3>
        <p>St George’s Lupset Ltd is an equal opportunities employer.  All applicants will be considered on the basis of suitability for the post, regardless of sex, race, marital status, religion, disability, or sexual orientation.</p>
      </div>

      <h3>Declaration of accuracy</h3>
      {% include fields/check.html type="text" name="accuracy" label="I declare that all the information given by me in this application is accurate.  I understand that any false information given in this application may render an offer of employment invalid and may lead to termination of employment." %}




      <!-- recaptcha and submit -->
      <h3>Confirm that you’re human</h3>
      <p>This helps us prevent spam or other automated applications.</p>
      <div class="g-recaptcha" data-sitekey="6LdNn1AUAAAAAA-VLy7CCzufqQi7EhPyoWQwcHIM"></div>

      <div class="form-status alert"></div>
      <div class="tab-footer-navigation">
        <a data-tab="experience" class="button white back">Previous</a>
        <input type="submit" value="Submit" class="white button"/>
      </div>
    </div>
    <div class="slide"></div>

  </form>