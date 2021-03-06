# MosaicBackend

@LuisToro-v and I build an instagram backend api for shared photo viewing.

# Vision

- Mosaic is a photo sharing application, that removes the visual clutter of comments and likes. The homepage (accesible by any user non-authenticated & authenticated) displays a mosaic of most recent images on the platform. On hover over an image, it's poster's username is diplayed on the bottom right corner of the photo. Clicking on the username will bring you to mosaic.com/:username. This user's mosaic of photos resembles the home page.

![img](https://i2.wp.com/css-tricks.com/wp-content/uploads/2011/07/seamless.png?ssl=1)

- This vision was influenced by a short time constraint, and our inexperience with routing, and node's pg-promise. We learned tons about these exciting technologies, version control and kanban project management.

# Challenges we faced.

- KnexJS does not support integer arrays within its DDL.

- Limited information returned from the database when deleting. It would be nice to give some verbose information to the front end.

- Adding robustness to endpoints in several identified edge cases.

# API

## DELETE USER http://localhost:3000/deleteUser

## GET Username mosaic http://localhost:3000/:username

## PUT photo to user's mosaic http://localhost:3000/addPhoto

## DELETE photo from user's mosaic http://localhost:3000/deletePhoto/

## GET universal mosaic photos in chronological order http://localhost:3000/

## PUT (Create) new user http://localhost:3000/createUser
