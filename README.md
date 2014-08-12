API needs
---

###Existing:

`/api/1/authors/`
> Has: `GET`, `POST`  
> Needs: `PUT`, `PATCH`, `DELETE`

`/api/1/categories/`
>Has: `GET`, `POST`  
>Needs: `PUT`, `PATCH`, `DELETE`

`/api/1/content_types`  &rarr;	 **do we need this(?)**
> Has: `GET`, `POST`  
> Needs: `PUT`, `PATCH`, `DELETE`

`/api/1/photos/`
> Has: `GET`, `POST`  
> Needs: `PUT`, `PATCH`, `DELETE` **(?)**

`/api/1/publishables/`
> Has: `GET`, `POST`  
> Needs: `PUT`, `PATCH`, `DELETE`

`/api/1/users`
> Has: `GET`  
> Needs: `POST`, `PUT`, `PATCH`, `DELETE`

###Needs:

`/api/1/permissions/` **(?)**
> Needs:
>> `GET`: a list of all permissions  
>> `POST`, `PUT`, `PATCH`, `DELETE`

> Why: Need an endpoint to get a list of **all** permissions **(?)**

`/api/1/permissions/group/:id` **(?)**
> `GET`: permissions for a user_group (ie: superadmin, editor, etc) based on id;  
> `POST`, `PUT`, `PATCH`, `DELETE`


`/api/1/permissions/user/:id` **(?)**
> `GET`: permissions for a user based on id  
> `POST`, `PUT`, `PATCH`, `DELETE`

---

###Questions:
* How are authors/users/profiles/etc related?  


---

###Needs:
* Permission modeling and integration
* Save as draft / auto save for all input types
* Figure out a life cycle for user generated content
  * All uploaded content needs a state 
* Need CRUD with error checking for relating content items to publishables/etc.
* Nuke photo formats **(?)**
