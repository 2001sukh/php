
## CHANGED PORTIONS IN LAB = 11-b

# Changes in routes.php 

- Prefix Addition: Added a "/11-b/" prefix to all existing routes in the code.

- Uniform Application: This modification was uniformly applied to all types of routes, including GET, POST, PATCH, and DELETE.

- Route Updates: As a result, each route, from basic pages like '/about' to more specific functions like '/notes/create', now starts with "/11-b/".

- Functionality and Controllers Unchanged: The core functionality and the controllers linked to these routes remain unchanged; the only aspect modified were the URL paths.


# Changes in index.php 

- Initial Setting: The original BASE_PATH was set as const BASE_PATH = __DIR__.'/../';. This pointed to the parent directory of the current directory.

- Modification Made: I changed it to const BASE_PATH = __DIR__.'/';. This new setting points to the current directory where index.php is located.


# Changes in nav.php

- Home Link Path Change: I modified the Home link's href attribute from "/" to "/11-b/". This change redirects the Home link to the "/11-b/" path.

- Altered Paths for Other Links: For the About, Notes, and Contact links, I removed the leading slashes from their href attributes. Originally set as "/about", "/notes", and "/contact", I changed them to "about", "notes", and "contact", making the paths relative to the current directory.