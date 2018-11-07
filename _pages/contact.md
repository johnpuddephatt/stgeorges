---
title: Contact
layout: page
hidden: false
description: Whether you want to ask us something, tell us something, or get help planning a visit to us, you’ll find the information you need below.
date: 2018-05-09 15:50:54 +0000
tabs:
- title: 'Contact details'
  content: |-
    ## Contact our centre

    Telephone: 01924 369631

    Email: [info@stgeorgeslupset.org.uk](mailto:info@stgeorgeslupset.org.uk)

    Or call in and see us:

    <address>
      St George's Community Centre<br />
      Broadway<br />
      Lupset<br />
      Wakefield<br />
      West Yorkshire<br />
      WF2 8AA<br /><br />
    </address>


    You can also stay up to date by finding us on [Facebook](http://www.facebook.com/StGeorgesCommunityCentre) or following us on [Twitter](http://twitter.com/stgeorgeslupset).

    ## Contact our nurseries

    Contact details for each of our nurseries can be found on their individual pages:

    * [Childcare @ Broadway](/nurseries/broadway)
    * [Childcare @ Sandal](/nurseries/sandal)
    * [Childcare @ St. Swithun’s](/nurseries/stswithuns)
    * [Childcare @ Sunbeam](/nurseries/sunbeam)


- title: 'Finding us'
  content: |-
    St George's Community Centre is located in Lupset, Wakefield. Situated in between Leeds, Pontefract, Barnsley, Huddersfield and Halifax, there is easy access from the M1, M62 and M606.

    There are two train stations nearby: Westgate Train Station and Dewsbury Train Station. From both stations there are convenient bus links to the centre.
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2363.6537768595276!2d-1.5386839843188318!3d53.67097258004832!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x487966ce5e9786c3%3A0xe481f7a560b8b6c4!2sSt+George&#39;s+Community+Centre!5e0!3m2!1sen!2suk!4v1507031083283" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
- title: 'Send us a message'
  content: |-
    <form action="https://form.letsdance.agency/vzMz7DYk" method="POST">    
      <input type="text" name="_subject" hidden value="Enquiry from St George’s website"/>
      <label for="form-name">Name
      <input type="text" name="name" id="form-name" placeholder="Enter your name" required/>
      </label>
      <label for="form-email">Email
      <input type="email" name="_replyto" id="form-email" placeholder="Enter your email address" required/>
      </label>
      <label for="form-phone">Phone number
      <input type="number" name="phone" id="form-phone" placeholder="Enter your phone number (optional)"/>
      </label>
      <label for="form-type">My enquiry is about</label>
      <select name="type" id="form-type">
        <option value="" disabled selected>Please select...</option>
        <option value="Childcare">Childcare and early education</option>
        <option value="Learning and employability">Learning and employability</option>
        <option value="Wellbeing">Wellbeing</option>
        <option value="Young people’s activities">Young people’s activities</option>
        <option value="The cafe">The Cafe</option>
        <option value="Room hire">Room Hire</option>
        <option value="Minibus hire">Minibus Hire</option>
        <option value="Volunteering">Volunteering</option>
        <option value="Other">Other</option>
      </select>
      <div class="alert" id="childcare-alert"></div>
      <input name="_cc" type="hidden" id="form-cc" />
      <label for="form-message">Message</label>
      <textarea type="number" name="message" id="form-message" placeholder="Enter your message"></textarea>
      <div class="g-recaptcha" data-sitekey="6LdNn1AUAAAAAA-VLy7CCzufqQi7EhPyoWQwcHIM"></div>
      <input type="submit" value="Send" class="button"/>
    </form>
    <script type="text/javascript">
      var contactType = document.querySelector('#form-type');
      var formCc = document.querySelector('#form-cc');
      contactType.addEventListener("change", function(){
        if(this.value == 'Childcare') {
          formCc.value = 'childcare@stgeorgeslupset.co.uk';
        }
        else {
          formCc.value = '';
        }
      });
    </script>
---