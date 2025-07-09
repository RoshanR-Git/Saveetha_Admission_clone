# Saveetha_Admission_clone
## Date: 09.07.2025

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SAVEETHA ENGINEERING COLLEGE - ADMISSION</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <img src="poster.jpg" class="poster" alt="background" />
  
  <div class="form-container">
    <form class="form">
      <h1>Admission Open 2025</h1>

      <input type="text" placeholder="Enter Name*" class="input" required />
      <input type="email" placeholder="Enter Email Address*" class="input" required />
      
      <div class="phone-container">
        <select class="country-code">
          <option>+91</option>
          <option>+87</option>
          <option>+603</option>
          <option>+1</option>
          <option>+66</option>
        </select>
        <input type="text" placeholder="Enter Mobile Number*" maxlength="10" class="mobile" required />
      </div>

      <input type="password" placeholder="Any password of Your Choice" maxlength="8" class="input" required />
      <input type="text" placeholder="State*" class="input" required />
      <input type="text" placeholder="City*" class="input" required />
      <input type="text" placeholder="Course*" class="input" required />
      <input type="text" placeholder="Specialization*" class="input" required />

      <div class="captcha-container">
        <input type="text" placeholder="14eH7I" class="captcha" readonly />
        <input type="text" placeholder="Enter Captcha*" class="input" required />
      </div>

      <label class="consent">
        <input type="checkbox" required />
        I authorise Saveetha Engineering College & its representatives to contact me with updates and notifications.
      </label>

      <button type="submit" class="submit">APPLY NOW ➤</button>

      <h4>Already Have an Account? <a href="#">Login</a></h4>
      <h4><a href="#">Resend Verification Email</a></h4>
    </form>
  </div>
</body>
</html>
```
## CSS Code:
```
* 
{
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

html, body 
{
  margin: 0;
  padding: 0;
  min-height: 100%;
  width: 100%;
  overflow-x: hidden;
  overflow-y: auto;
}

.poster 
{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -1;
}

.form-container 
{
  display: flex;
  justify-content: flex-end;
  padding: 50px 5%;
  height: auto;
  min-height: 100vh;
}

.form 
{
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(10px);
  padding: 30px 40px;
  border-radius: 10px;
  width: 400px;
  display: flex;
  flex-direction: column;
  gap: 15px;
  color: white;
  margin-top: 20px;
  margin-bottom: 40px;
}

h1 
{
  color: #ff8400;
  text-align: center;
}

.input, .mobile, .country-code, .captcha 
{
  height: 40px;
  border-radius: 5px;
  border: none;
  padding: 10px;
  font-size: 15px;
  width: 100%;
}

.country-code 
{
  width: 30%;
}

.phone-container, .captcha-container 
{
  display: flex;
  gap: 10px;
}

.captcha 
{
  background: #e0e0e0;
  text-align: center;
  font-weight: bold;
  pointer-events: none;
}

.consent 
{
  font-size: 13px;
  display: flex;
  gap: 10px;
  align-items: center;
  color: white;
}

.submit 
{
  background-color: #ff8400;
  color: white;
  font-weight: bold;
  border: none;
  padding: 10px;
  border-radius: 6px;
  cursor: pointer;
  transition: background 0.3s;
}

.submit:hover 
{
  background-color: #e67300;
}

h4 
{
  text-align: center;
  margin: 5px 0;
  font-size: 14px;
  color: white;
}

a 
{
  color: #ff8400;
  text-decoration: underline;
}

@media screen and (max-width: 768px) 
{
  .form-container 
  {
    justify-content: center;
    padding: 30px 20px;
  }

  .form 
  {
    width: 90%;
    padding: 25px;
  }

  .phone-container, .captcha-container 
  {
    flex-direction: column;
  }

  .country-code 
  {
    width: 100%;
  }
}

@media screen and (max-width: 480px) 
{
  h1 
  {
    font-size: 22px;
  }

  .input, .mobile, .country-code, .captcha 
  {
    font-size: 14px;
    padding: 8px;
  }

  .submit 
  {
    font-size: 14px;
    padding: 8px;
  }

  h4 
  {
    font-size: 12px;
  }
}
```
## Output:
![Screenshot 2025-07-09 221922](https://github.com/user-attachments/assets/4c2896b4-e9ad-493c-8c82-89c89aa47722)

## LiveWebpage:

## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
