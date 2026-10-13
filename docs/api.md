# Routes and interactions

## Server API

There is no server-side API in this repository. The project consists of static HTML files and images. It defines no HTTP handlers, JSON endpoints, form submission targets, API authentication, or data contract.

## Page entry points

| Page | Browser interaction |
| --- | --- |
| Assignment_14_Bootstrap/Task_1.html | Displays a course card. Enroll Now is an anchor with href="#"; it does not submit or navigate to an enrollment service. |
| Assignment_14_Bootstrap/Task_2.html | Displays a three-image Bootstrap carousel with indicators and previous/next controls. Bootstrap's JavaScript bundle handles carousel behavior in the browser. |
| Assignment_14_Bootstrap/Task_3.html | Displays navigation, a Courses dropdown, placeholder links, and a button that opens a login modal. |

## Login modal

The modal contains email and password inputs for presentation. The form has no action URL, no submit event handler, and no backend. The Login footer button is not wired to authentication. Do not enter real credentials, and do not describe this example as a working login system.

## Browser assets

Each page loads Bootstrap 5.3.2 from jsDelivr using CSS and JavaScript bundle URLs with integrity metadata. The HTML also loads images from the local media directory. These are static asset requests, not a project API.
