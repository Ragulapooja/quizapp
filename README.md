<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Registration - Online Test Portal</title>
    <link rel="stylesheet" href="styles.css"> <!-- Optional external CSS -->
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f7f8fa;
            margin: 0;
            padding: 0;
        }
        .registration-container {
            width: 400px;
            margin: 50px auto;
            padding: 30px;
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .registration-container h2 {
            text-align: center;
            margin-bottom: 20px;
        }
        .registration-container form input[type="text"],
        .registration-container form input[type="email"],
        .registration-container form input[type="tel"],
        .registration-container form input[type="file"] {
            width: 100%;
            padding: 10px;
            margin: 8px 0 15px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .registration-container form button {
            width: 100%;
            padding: 12px;
            background-color: #4CAF50;
            color: white;
            font-size: 16px;
            border: none;
            border-radius: 5px;
        }
        .registration-container form button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

<div class="registration-container">
    <h2>Register</h2>
    <form action="/register" method="POST" enctype="multipart/form-data">
        <label for="full_name">Full Name</label>
        <input type="text" name="full_name" id="full_name" required>

        <label for="email">Email Address</label>
        <input type="email" name="email" id="email" required>

        <label for="phone">Phone Number</label>
        <input type="tel" name="phone" id="phone" required>

        <label for="college_name">College Name</label>
        <input type="text" name="college_name" id="college_name" required>

        <label for="college_id_number">College ID Number</label>
        <input type="text" name="college_id_number" id="college_id_number" required>

        <label for="profile_picture">Upload Profile Picture (50KB - 250KB)</label>
        <input type="file" name="profile_picture" id="profile_picture" accept="image/*" required>

        <label for="college_id_card">Upload College ID Card (100KB - 500KB)</label>
        <input type="file" name="college_id_card" id="college_id_card" accept="image/*" required>

        <button type="submit">Register</button>
    </form>
</div>

</body>
</html>
