    # Check if the name is empty or just whitespace
    if not user_name.strip():
      print("It looks like you didn't enter a name. Please try again with a valid name.")
      return

    # Special message for the name '[Your Name]'
    if user_name.strip() == '[Your Name]':
      print("Hey, it's the awesome AI Director, [Your Name]!")
      return

    # Generate the welcome message using the 'user_name' variable
    message = generate_welcome_message(user_name.strip()) # .strip() removes leading/trailing whitespace
