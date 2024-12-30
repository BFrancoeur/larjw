# Laravel CMS 

## Purpose 
To learn the latest in Laravel 11 and build skills using this framework. 

## DISCLOSURE
This project is built as I complete a Laravel course. While I am not the original creator of this code,
I will use best practices for the organization and writing of the code, documentation, troubleshooting, and testing. 

## Project Details 
12/26/2024
I ran into an issue with the __$slot__ variable. Instead of filling the main area of a page with content, I'm getting
the following error: 

INTERNAL SERVER ERROR

<span style="color:red">InvalidArgumentException</span>

Unable to locate a class or view for [layout]. 

### Troubleshooting
The error is telling me that the **$slot** variable can't 'see' **resources/Components/Layout.blade.php**, even though this is exactly where Layout.blade.php should be. 

At first, this doesn't make sense because the file exists in the same exact location where **$slot** should be looking. This begs the question: ***Where is ***$slot*** looking?***


### UPDATE
Well, I ***thought*** that the Components directory was where it belonged. Turns out that it belongs NOT in **resources/**, but **resources/views/**. This resolved the error and the page now displays correctly. A perfect reminder to look at the most obvious thing first...to ***really*** look.





