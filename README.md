# amazon-lex-overview

Below are the step for a quick Amazon Lex demo

**Prerequisite**
  
  1. Login to AWS account, and switch to us-east-1 region

  2. Search for Amazon Lex, and click 

  3. Under Bot section click Create

**Design & Deploy Lex Bot**
1. Boot Name - booking_a_table

2. Intent Name - reserve_a_table

3. Define custom slot type (hotel_name) with values - Taj, Aura, WareHouse, VegTreat

4. Define slots
    - bookingdate - AMAZON.DATE - On what date you want me to book a table?
    - bookingtime - AMAZON.TIME - At what time you want me to book a table?
    - numberofpeople - AMAZON.NUMBER - How many people will join you?
    - restaurantname - hotel_name - In which hotel you want to book?

5. Confirmation prompt 
    - Check Confirmation prompt 
    - Confirm - Are you sure you want to book a table at {restaurantname} for {bookingdate} at {bookingtime}?
    - Cancel (if the user says "no") - Your reservation will cancelled. Thank you!
