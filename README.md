# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>HTML5 Page with Registration Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        table, th, td {
            border: 1px solid #000;
        }
        th, td {
            padding: 8px;
            text-align: left;
        }
        form {
            margin-top: 20px;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            margin: 10px 0;
        }
        label {
            font-weight: bold;
        }
        .required {
            color: red;
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to Our Web Page</h1>
    </header>

    <!-- Ordered List with Roman Numerals -->
    <section>
        <h2>Important Points</h2>
        <ol type="I">
            <li>Research is critical to success.</li>
            <li>Investing in skills is key to long-term growth.</li>
            <li>Networking and building relationships.</li>
        </ol>
    </section>

    <!-- External Image from Pexels -->
    <section>
        <h2>Our Featured Image</h2>
        <img src="https://images.pexels.com/photos/3412072/pexels-photo-3412072.jpeg" alt="Beautiful Landscape" style="width:100%; height:auto;">
    </section>

    <!-- Table of Contacts -->
    <section>
        <h2>Contact List</h2>
        <table>
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>John Doe</td>
                    <td>123 Main St, Cityville</td>
                    <td>+234 802 123 4567</td>
                    <td>johndoe@example.com</td>
                </tr>
                <tr>
                    <td>Jane Smith</td>
                    <td>456 Elm St, Townsville</td>
                    <td>+234 802 987 6543</td>
                    <td>janesmith@example.com</td>
                </tr>
                <tr>
                    <td>Michael Johnson</td>
                    <td>789 Oak St, Suburbia</td>
                    <td>+234 802 564 8974</td>
                    <td>michaelj@example.com</td>
                </tr>
                <tr>
                    <td>Linda Clark</td>
                    <td>101 Pine St, Uptown</td>
                    <td>+234 802 349 8234</td>
                    <td>lindac@example.com</td>
                </tr>
                <tr>
                    <td>James Walker</td>
                    <td>202 Cedar St, Downtown</td>
                    <td>+234 802 874 2223</td>
                    <td>jamesw@example.com</td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- Registration Form -->
    <section>
        <h2>Registration Form</h2>
        <form action="#" method="POST">
            <!-- Name Field -->
            <label for="name">Full Name <span class="required">*</span></label>
            <input type="text" id="name" name="name" placeholder="Enter your full name" required>

            <!-- Email Field -->
            <label for="email">Email <span class="required">*</span></label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required>

            <!-- Password Field -->
            <label for="password">Password <span class="required">*</span></label>
            <input type="password" id="password" name="password" placeholder="Enter your password" required minlength="8">

            <!-- Date Field -->
            <label for="dob">Date of Birth <span class="required">*</span></label>
            <input type="date" id="dob" name="dob" required>

            <!-- Dropdown Menu -->
            <label for="country">Country</label>
            <select id="country" name="country">
                <option value="nigeria">Nigeria</option>
                <option value="usa">United States</option>
                <option value="uk">United Kingdom</option>
                <option value="canada">Canada</option>
            </select>

            <!-- Radio Buttons for Gender -->
            <fieldset>
                <legend>Gender <span class="required">*</span></legend>
                <label><input type="radio" name="gender" value="male" required> Male</label><br>
                <label><input type="radio" name="gender" value="female"> Female</label><br>
                <label><input type="radio" name="gender" value="other"> Other</label>
            </fieldset>

            <!-- Checkboxes for Interests -->
            <fieldset>
                <legend>Interests</legend>
                <label><input type="checkbox" name="interests" value="sports"> Sports</label><br>
                <label><input type="checkbox" name="interests" value="technology"> Technology</label><br>
                <label><input type="checkbox" name="interests" value="music"> Music</label><br>
            </fieldset>

            <!-- Submit Button -->
            <button type="submit">Register</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Our Company</p>
    </footer>

</body>
</html>
