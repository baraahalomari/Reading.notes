# Status Codes Based On REST Methods


In your own words, describe what each group of status code represents:

>  100’s = telling the client that its request will fail before they start sending the body

> 200’s = this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

> 300’s = They tell the client that the resource they are requesting isn’t available at the expected location anymore.

> 400’s =They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication.

> 500’s = These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

## What is a status code 202?

These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.


## What is a status code 308?

308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

## What code would you use if an update didn’t return data to a client?

204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

## What code would you use if a resource used to exist but no longer does?
410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

## What is the ‘Forbidden’ status code?
403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.
