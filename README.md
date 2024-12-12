# React Router Dom v6 Unexpected Route Behavior

This repository demonstrates a common error in React Router Dom v6: unexpected route behavior when a route is missing for a given path.  The application renders a default component (Home in this case) rather than throwing an error or displaying a 404 page.

## Bug Description:
The application renders the Home component even if you try to navigate to '/contact'.  This is because no route is defined for '/contact' in the Routes component. In earlier versions of React Router, this might have caused an error; now, it leads to unexpected behavior.

## Solution:
Add a route for '/contact' to handle this case.