# Tips for NestJS

- Install globally - `npm install -g @nestjs/cli`
- Build a project - `nest new PROJECT-NAME && cd PROJECT-NAME && yarn run start`

## Tips
- Controller = Request Manager
- Module = Task Manager
- No need nodemon

## Architecture
- Decorators = @Module, @Controllers, @Get or @Providers
- When you run, It will create a dist - build folder

### Controller
- @Controller()
- Is a class manager
- No need `new AppController().getHello()` for example
- No need create a router to call AppController - Manual configuration was necessary on Express
- Controller do it for yourself
- @Get is a route - for example

### Module
- @Module
- It is a responsible for receiving information about class
- Controllers is a classes managers
- Providers is a injectable services like a @Injectable on AppService
