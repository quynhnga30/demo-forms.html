# demo-forms.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>forms</title>
</head>
<body>
    <h2>Text input fields</h2>
    <from>
      <label for="fname">First name:</label>
    <br>
      <input type="text" id="fname"
    name="fname" value="John"><br>
      <label for="lname">Last name:</label>
    <br>
      <input type="text" id="lname"
    name="lname" value="Doe">
     </from>
     <p>Note that the form itself is not visible.</p>
     <p>Also note that the default width of text input fields í 20 character.</p>
</body>
</html>
-----
<!DOCTYPE html>
<html>
<body>

<h2>Radio Buttons</h2>

<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form> 

</body>
</html>
-----
<!DOCTYPE html>
<html>
<body>

<h2>Checkboxes</h2>
<p>The <strong>input type="checkbox"</strong> defines a checkbox:</p>

<form action="/action_page.php">
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label><br><br>
  <input type="submit" value="Submit">
</form> 

</body>
</html>
-----
<!DOCTYPE html>
<html>
<body>

<h2>HTML Forms</h2>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>

</body>
</html>
----
<!DOCTYPE html>
<html>
<body>

<h2>The name Attribute</h2>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" value="John"><br><br>
  <input type="submit" value="Submit">
</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>

<p>Notice that the value of the "First name" field will not be submitted, because the input element does not have a name attribute.</p>

</body>
</html
----
<!DOCTYPE html>
<html>
<body>

<h2>HTML Forms</h2>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>

</body>
</html>
---
Phần tử input:
<!DOCTYPE html>
<html>
<body>

<h2>The input Element</h2>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Phần tử select
<!DOCTYPE html>
<html>
<body>

<h2>The select Element</h2>

<p>The select element defines a drop-down list:</p>

<form action="/action_page.php">
  <label for="cars">Choose a car:</label>
  <select id="cars" name="cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="fiat">Fiat</option>
    <option value="audi">Audi</option>
  </select>
  <input type="submit">
</form>

</body>
</html>
Phần tử textareosystem
<!DOCTYPE html>
<html>
<body>

<h2>Textarea</h2>
<p>The textarea element defines a multi-line input field.</p>

<form action="/action_page.php">
  <textarea name="message" rows="10" cols="30">The cat was playing in the garden.</textarea>
  <br><br>
  <input type="submit">
</form>

</body>
</html>
Phần tử button
<!DOCTYPE html>
<html>
<body>

<h2>The button Element</h2>

<button type="button" onclick="alert('Hello World!')">Click Me!</button>

</body>
</html>
Phần tử fieldset và legend
<!DOCTYPE html>
<html>
<body>

<h2>Grouping Form Data with Fieldset</h2>

<p>The fieldset element is used to group related data in a form, and the legend element defines a caption for the fieldset element.</p>

<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>

</body>
</html>
Phần tử datalist
<!DOCTYPE html>
<html>
<body>

<h2>The datalist Element</h2>

<p>The datalist element specifies a list of pre-defined options for an input element.</p>

<form action="/action_page.php">
  <input list="browsers" name="browser">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
  <input type="submit">
</form>

<p><b>Note:</b> The datalist tag is not supported in Safari prior version 12.1.</p>

</body>
</html>
Phần tử output
<!DOCTYPE html>
<html>
<body>

<h2>The output Element</h2>
<p>The output element represents the result of a calculation.</p>

<form action="/action_page.php"
oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range" id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form>

<p><strong>Note:</strong> The output element is not supported in Edge prior version 13.</p>

</body>
</html>

<!DOCTYPE html>
<html>
<body>

<h2>Text field</h2>
<p>The <strong>input type="text"</strong> defines a one-line text input field:</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>

<p>Note that the form itself is not visible.</p>
<p>Also note that the default width of a text field is 20 characters.</p>

</body>
</html>
Nhập mật khẩu
<!DOCTYPE html>
<html>
<body>

<h2>Password field</h2>

<p>The <strong>input type="password"</strong> defines a password field:</p>

<form action="/action_page.php">
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="pwd">Password:</label><br>
  <input type="password" id="pwd" name="pwd"><br><br>
  <input type="submit" value="Submit">
</form>

<p>The characters in a password field are masked (shown as asterisks or circles).</p>

</body>
</html>
Loại đầu vào Gửi
<!DOCTYPE html>
<html>
<body>

<h2>Submit Button</h2>

<p>The <strong>input type="submit"</strong> defines a button for submitting form data to a form-handler:</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 

<p>If you click "Submit", the form-data will be sent to a page called "/action_page.php".</p>

</body>
</html>
biểu mẫu mặc định 
<!DOCTYPE html>
<html>
<body>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit">
</form> 

</body>
</html>
Đặt lại loại đầu vào
<!DOCTYPE html>
<html>
<body>

<h2>Reset Button</h2>

<p>The <strong>input type="reset"</strong> defines a reset button that resets all form values to their default values:</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
  <input type="reset">
</form> 

<p>If you change the input values and then click the "Reset" button, the form-data will be reset to the default values.</p>

</body>
</html>
Loại đầu vào Radio
<!DOCTYPE html>
<html>
<body>

<h2>Radio Buttons</h2>

<p>The <strong>input type="radio"</strong> defines a radio button:</p>

<p>Choose your favorite Web language:</p>
<form action="/action_page.php">
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label><br><br>
  <input type="submit" value="Submit">
</form> 

</body>
</html>
Hộp kiểm loại đầu vào
<!DOCTYPE html>
<html>
<body>

<h2>Checkboxes</h2>
<p>The <strong>input type="checkbox"</strong> defines a checkbox:</p>

<form action="/action_page.php">
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label><br><br>
  <input type="submit" value="Submit">
</form> 

</body>
</html>
Nút loại đầu vào
<!DOCTYPE html>
<html>
<body>

<h2>Input Button</h2>

<input type="button" onclick="alert('Hello World!')" value="Click Me!">

</body>
</html>
Loại đầu vào Màu sắc
<!DOCTYPE html>
<html>
<body>

<h2>Show a Color Picker</h2>

<p>The <strong>input type="color"</strong> is used for input fields that should contain a color.</p>

<form action="/action_page.php">
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor" value="#ff0000">
  <input type="submit" value="Submit">
</form>

<p><b>Note:</b> type="color" is not supported in Internet Explorer 11 or Safari 9.1 (or earlier).</p>

</body>
</html>
Loại đầu vào Ngày
<!DOCTYPE html>
<html>
<body>

<h2>Date Field</h2>

<p>The <strong>input type="date"</strong> is used for input fields that should contain a date.</p>

<form action="/action_page.php">
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday">
  <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> type="date" is not supported in Internet Explorer 11 or prior Safari 14.1.</p>

</body>
</html>
Loại đầu vào Ngày giờ-cục bộ
<!DOCTYPE html>
<html>
<body>

<h2>Local Date Field</h2>

<p>The <strong>input type="datetime-local"</strong> specifies a date and time input field, with no time zone.</p>

<form action="/action_page.php">
  <label for="birthdaytime">Birthday (date and time):</label>
  <input type="datetime-local" id="birthdaytime" name="birthdaytime">
  <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> type="datetime-local" is not supported in Internet Explorer 11 or prior Safari 14.1.</p>

</body>
</html>
Loại đầu vào Email

<!DOCTYPE html>
<html>
<body>

<h2>Email Field</h2>

<p>The <strong>input type="email"</strong> is used for input fields that should contain an e-mail address:</p>

<form action="/action_page.php">
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email">
  <input type="submit" value="Submit">
</form>

</body>
</html>
Tệp loại đầu vào
<!DOCTYPE html>
<html>
<body>

<h1>File upload</h1>

<p>Show a file-select field which allows a file to be chosen for upload:</p>
<form action="/action_page.php">
  <label for="myfile">Select a file:</label>
  <input type="file" id="myfile" name="myfile"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Loại đầu vào bị ẩn
<!DOCTYPE html>
<html>
<body>

<h1>A Hidden Field (look in source code)</h1>

<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="hidden" id="custId" name="custId" value="3487">
  <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> The hidden field is not shown to the user, but the data is sent when the form is submitted.</p>

</body>
</html>
Loại đầu vào Tháng
<!DOCTYPE html>
<html>
<body>

<h2>Month Field</h2>

<p>The <strong>input type="month"</strong> allows the user to select a month and year.</p>

<form action="/action_page.php">
  <label for="bdaymonth">Birthday (month and year):</label>
  <input type="month" id="bdaymonth" name="bdaymonth">
  <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> type="month" is not supported in Firefox, Safari, or Internet Explorer 11.</p>

</body>
</html>
Số loại đầu vào
<!DOCTYPE html>
<html>
<body>

<h2>Number Field</h2>

<p>The <strong>input type="number"</strong> defines a numeric input field.</p>

<p>You can use the min and max attributes to add numeric restrictions in the input field:</p>

<form action="/action_page.php">
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
  <input type="submit" value="Submit">
</form>

</body>
</html>
Hạn chế đầu vào
<!DOCTYPE html>
<html>
<body>

<h2>Numeric Steps</h2>

<p>Depending on browser support: Fixed steps will apply in the input field.</p>

<form action="/action_page.php">
  <label for="quantity">Quantity:</label>
  <input type="number" id="quantity" name="quantity" min="0" max="100" step="10" value="30">
  <input type="submit" value="Submit">
</form>

</body>
</html>
---thuộc tính đầu vào
Thuộc tính giá trị
<!DOCTYPE html>
<html>
<body>

<h1>The input value attribute</h1>

<p>The value attribute specifies an initial value for an input field:</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính chỉ đọc
<!DOCTYPE html>
<html>
<body>

<h1>The input readonly attribute</h1>

<p>The readonly attribute specifies that an input field should be read-only (cannot be changed):</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" readonly><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính bị vô hiệu hóa
<!DOCTYPE html>
<html>
<body>

<h1>The input disabled attribute</h1>

<p>The disabled attribute specifies that an input field should be disabled (unusable and un-clickable):</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" disabled><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính kích thước
<!DOCTYPE html>
<html>
<body>

<h1>The input size attribute</h1>

<p>The size attribute specifies the width (in characters) of an input field:</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" size="4"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính maxlength
<!DOCTYPE html>
<html>
<body>

<h1>The input maxlength attribute</h1>

<p>The maxlength attribute specifies the maximum number of characters allowed in an input field:</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" maxlength="4" size="4"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính tối thiểu và tối đa
<!DOCTYPE html>
<html>
<body>

<h1>The input min and max attributes</h1>

<p>The min and max attributes specify the minimum and maximum values for an input element.</p>

<form action="/action_page.php">
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5"><br><br>

  <input type="submit" value="Submit">
</form>

</body>
</html>
Nhiều thuộc tính
<!DOCTYPE html>
<html>
<body>

<h1>The input multiple attributes</h1>

<p>The multiple attribute specifies that the user is allowed to enter more than one value in an input field.</p>

<form action="/action_page.php">
  <label for="files">Select files:</label>
  <input type="file" id="files" name="files" multiple><br><br>
  <input type="submit" value="Submit">
</form>

<p>To select multiple files, hold down the CTRL or SHIFT key while selecting.</p>

</body>
</html>
Thuộc tính mẫu
<!DOCTYPE html>
<html>
<body>

<h1>The input pattern attribute</h1>

<p>The pattern attribute specifies a regular expression that the input element's value is checked against.</p>

<form action="/action_page.php">
  <label for="country_code">Country code:</label>
  <input type="text" id="country_code" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code"><br><br>
  <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> The pattern attribute of the input tag is not supported in Safari 10 (or earlier).</p>

</body>
</html>
Thuộc tính trình giữ chỗ
<!DOCTYPE html>
<html>
<body>

<h1>The input placeholder attribute</h1>

<p>The placeholder attribute specifies a short hint that describes the expected value of an input field.</p>

<form action="/action_page.php">
  <label for="phone">Enter a phone number:</label>
  <input type="tel" id="phone" name="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính bắt buộc

<!DOCTYPE html>
<html>
<body>

<h1>The input required attribute</h1>

<p>The required attribute specifies that an input field must be filled out before submitting the form.</p>

<form action="/action_page.php">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>
  <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> The required attribute of the input tag is not supported in Safari prior version 10.1.</p>

</body>
</html>
Thuộc tính bước
<!DOCTYPE html>
<html>
<body>

<h1>The input step attribute</h1>

<p>The step attribute specifies the legal number intervals for an input element.</p>

<form action="/action_page.php">
  <label for="points">Points:</label>
  <input type="number" id="points" name="points" step="3">
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính lấy nét tự động
<!DOCTYPE html>
<html>
<body>

<h1>The input autofocus attribute</h1>

<p>The autofocus attribute specifies that the input field should automatically get focus when the page loads.</p>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" autofocus><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
Thuộc tính chiều cao và chiều rộng
<!DOCTYPE html>
<html>
<body>

<h1>The input height and width attributes</h1>

<p>The height and width attributes specify the height and width of an input type="image" element.</p>

<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>

<p><b>Note:</b> The input type="image" sends the X and Y coordinates of the click that activated the image button.</p>

</body>
</html>
thuộc tính danh sách
<!DOCTYPE html>
<html>
<body>

<h1>The input list attribute</h1>

<p>The list attribute refers to a datalist element that contains pre-defined options for an input element.</p>

<form action="/action_page.php">
  <input list="browsers" name="browser">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
  <input type="submit" value="Submit">
</form>

<p><b>Note:</b> The datalist tag is not supported in Safari 12.0 (or earlier).</p>

</body>
</html>
Thuộc tính tự động hoàn thành
<!DOCTYPE html>
<html>
<body>

<h1>The autocomplete attribute</h1>

<p>The autocomplete attribute specifies whether or not an input field should have autocomplete enabled.</p>

<p>Fill in and submit the form, then reload the page to see how autocomplete works.</p>

<p>Notice that autocomplete is "on" for the form, but "off" for the e-mail field!</p>

<form action="/action_page.php" autocomplete="on">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>
--biểu mẫu
Thuộc tính biểu mẫu
<!DOCTYPE html>
<html>
<body>

<h1>The input form attribute</h1>

<p>The form attribute specifies the form an input element belongs to.</p>

<form action="/action_page.php" id="form1">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
</form>

<p>The "Last name" field below is outside the form element, but still part of the form.</p>

<label for="lname">Last name:</label>
<input type="text" id="lname" name="lname" form="form1">

</body>
</html>
Thuộc tính formaction
<!DOCTYPE html>
<html>
<body>

<h1>The input formaction attribute</h1>

<p>The formaction attribute specifies the URL of a file that will process the input when the form is submitted.</p>

<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formaction="/action_page2.php" value="Submit as Admin">
</form>

</body>
</html>
Thuộc tính formenctype
<!DOCTYPE html>
<html>
<body>

<h1>The input formenctype attribute</h1>

<p>The formenctype attribute specifies how the form data should be encoded when submitted.</p>

<form action="/action_page_binary.asp" method="post">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formenctype="multipart/form-data" value="Submit as Multipart/form-data">
</form>

</body>
</html>
Thuộc tính formmethod
<!DOCTYPE html>
<html>
<body>

<h1>The input formmethod Attribute</h1>

<p>The formmethod attribute defines the HTTP method for sending form-data to the action URL.</p>

<form action="/action_page.php" method="get" target="_blank">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit using GET">
  <input type="submit" formmethod="post" value="Submit using POST">
</form>

</body>
</html>
Thuộc tính mục tiêu biểu mẫu
<!DOCTYPE html>
<html>
<body>

<h1>The input formtarget attribute</h1>

<p>The formtarget attribute specifies a name or a keyword that indicates where to display the response that is received after submitting the form.</p>

<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formtarget="_blank" value="Submit to a new window/tab">
</form>

</body>
</html>
Thuộc tính formnovalidate
<!DOCTYPE html>
<html>
<body>

<h1>The input formnovalidate attribute</h1>

<form action="/action_page.php">
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email" required><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formnovalidate="formnovalidate" value="Submit without validation">
</form>

<p><strong>Note:</strong> The formnovalidate attribute of the input tag is not supported in Safari 10 (or earlier).</p>

</body>
</html>
Thuộc tính không hợp lệ
<!DOCTYPE html>
<html>
<body>

<h1>The form novalidate attribute</h1>

<p>The novalidate attribute specifies that the form data should not be validated when submitted.</p>

<form action="/action_page.php" novalidate>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email" required><br><br>
  <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> The novalidate attribute of the form tag is not supported in Safari 10 (or earlier).</p>

</body>
</html>

