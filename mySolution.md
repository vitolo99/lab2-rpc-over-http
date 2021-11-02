# Web Engineering 2021-2022 / Lab2 RPC over HTTP

## Primary goal

In order to achieve the primary goal, I tried to build the code using gradelw following on the documentation of the last practice. But when building the project it starts building the client module so the build fails because it requires code derived from a wsdl file published by the server.

I searched online the way to apply the gradelw commands build and bootRun choosing the module of a proyect and I opened two differents terminals and in the first one: "./gradlew :server:build" and "./gradlew :server:bootRun". Then when the server is already running,  in the second one: "./gradlew :client:build" and "./gradlew :client:bootRun".

Then, it shows an error because the server response is implemented whit the "TODO()" option that is used to made you remember that the part when it is used hasn´t been correctly implemented yet. I replace that by a response, building a block harcoding the string "hola" in the translation element. In addition to that, i replaced the imput of the client request by "hello" and by building the Server side and the client side again, I obtained the required answer (> Task :client:bootRun: Result of translating [hello] is [Hola]).