# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > Create Read Update Delete

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > Create - Post,  Read - Get,  Update- Put,  Delete - Delete

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > object-relational mapping

04. Which two `HTTP` request types include a body?

  > Post and Put

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an ASYNCHRONOUS coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  >  , SYCHRONOUSE, ASYNCHRONOUS

06. What are the three types of data relationships? Provide an example of each.

  > One to One - one employee to one location they work
  One to Many - one customer to their many orders
  Many to Many - students to courses

07. What is middleware?

  > Middleware is the software that is the 'interpreter' between two main softwares. In our current week, Auth0 is our middleware. At my old job we had middleware that translated our baning information so that it could communicate to our customer's pos baning service.  In our reading called An intro to Javascript Middleware is described as a proxy for javascript objects.

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks.
The term Pipeline isn't in any of our reading material that I have been provided thus far, nor has anyone discussed it.
  > Totally guessing here, read my notes below. Client pipeline delivers requests from client, and servier returns responses it?
Found this on Mdn web docs
 Or you could be  referring to HTTP pipelineing. HTTP pipelining
Note: HTTP pipelining is not activated by default in modern browsers:

Buggy proxies are still common and these lead to strange and erratic behaviors that Web developers cannot foresee and diagnose easily.
Pipelining is complex to implement correctly: the size of the resource being transferred, the effective RTT that will be used, as well as the effective bandwidth, have a direct incidence on the improvement provided by the pipeline. Without knowing these, important messages may be delayed behind unimportant ones. The notion of important even evolves during page layout! HTTP pipelining therefore brings a marginal improvement in most cases only.
Pipelining is subject to the HOL problem.
For these reasons, pipelining has been superseded by a better algorithm, multiplexing, that is used by HTTP/2.

https://developer.mozilla.org/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x

   I reviewed all my notes, all readings, all labs and checkpoint directions and there is not mention of it. I searched future readings and found it here https://codeworksacademy.com/fs-student-guide/resources/wk8-9/04-Vue-Testing.html.
  Faster feedback loops
One of the primary problems with end-to-end (E2E) tests and development is that running the entire suite takes a long time. Typically, this is only done in continuous integration and deployment (CI/CD) pipelines. Modern E2E testing frameworks have helped to solve this by adding features like parallelization, which allows for CI/CD pipelines to often run magnitudes faster than before. In addition, when developing locally, the ability to selectively run a single test for the page you are working on while also providing hot reloading of tests can help to boost a developer’s workflow and productivity.

Visibility in headless mode
When end-to-end (E2E) tests are run in continuous integration / deployment pipelines, they are often run in headless browsers (i.e., no visible browser is opened for the user to watch). As a result, when errors occur, a critical feature that modern E2E testing frameworks provide 1st class support for is the ability to see snapshots and/or videos of your applications during various testing stages in order to provide insight into why errors are happening. Historically, it was tedious to maintain these integrations.

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

Summary: object that has a property called tag with the value of winter

SERVER SIDE - BACK END
1. Controller, constructor, I am not going to format it, know we start after the router line.
constructor(){
.get('', this.getItems)
2. ItemsController, getItems method
async getItems(request, response, next) {
            const query = request.query
            const items = await itemsService.getItems(query)
            response.send(items)
        } catch (error) {
            next(error)
        }
    }
}
3. ItemsService
 async getItems(query) {
        const items = await dbContext.Items.find(query)
        return items
    }
CLIENT SIDE - FRONT END
4. Controller, private function
function _drawItemsWithWinter() {
    let winterItems = data
    let content = ''
    items.find(wItem => content += caseObj.ListTemplate)
    setHTML('winter-list', content)
}

5. Items Service
setWinterItem(itemId) {
        let foundWinterItem = AppState.items.find(object => Obj.id == caseId)
        AppState.winterItems = foundCase
        returnv
    }

 


10. What is a ***virtual property***?

  >  Most (I would venture to day all) softwares have objects (in specific JS terms, and in general terms ) and those objects will have a unique identifier that is assigned that so the software, users, etc can track that that object through the system. In our current work, it is a property on a schema that comes from another schema. Here is my example: You have two items. A Main Item, and a Dependant Item that each have their own uinique identifier. In addition, the Depenant Item will have the Main Item's unique identifier as it is associated (related) to it. You can also see it as a Parent / Child relationship.
