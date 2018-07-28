# black-hole

the idea is to utilize graphql or maybe just http requests to summon React portals that allow for the next micro app to be loaded within an overseeing application shell.

black-hole(app shell) > REST/graphQL > react portal > micro app

## Ideas

Build a base layer app shell that keeps the mindset of a SPA. This is where we would allow for login functoins to live with in the context/redux state of the app shell. Each app within could call upon these global functions to do most of the inner logic they need. using the functions to pass that info back and make all REST/GraphQL requests in the app shell.

the App shell would also have it's own requests through REST/GraphQL to inject SSR micro apps into self summoning react portals. These portals would act as a routable page, but call the app internally. there could be some logic to cut out dependencies already cached and such in the REST call or GraphQL schema. Allowing for there to be little version collision over all. this is where we can tag in some logic for how the portals will be served to the app shell. Gaining the ability to add animations and such.

the micro apps would need to probably have some configuration on how and what to serve depending on the app shell's global state???
(still don't know what would all need to change, but i'm thinking not that much.)

## Disclaimer
I'm just throwing this stuff down here and plan to build on it later. I think there is a way to make this work it's just going to come from hard work and a lot of testing.
