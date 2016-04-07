# Standard
A few standard libraries we use for development

## LogitechF310
This is a static class that allows you to clarify references to controller buttons.
Eg. instead of `new Button(1)` you use `new Button(LogitechF310.A)`

## Installing

If your robot project (`workspace/robot`) is not a git project, this is very simple.
Just open the command line, navigate to `workspace/robot/src` and type the following
command: `git clone https://https://github.com/Team236/Standard.git standard`.

If your robot project is a git project, then you have to add it as a git submodule.
This is an experimental feature that hasn't existed for too long, so keep in mind
that it's not perfect for more complex purposes. For what we're doing, however, it's
perfect. Just navigate to `workspace/robot/src` and type the following commands:

`git submodule add https://github.com/Team236/Standard.git standard`

`git submodule init`

This will import the module and create unstaged changes. You
will have to commit this change, and commit the change whenever you update the
module.

After this, your tree should look like this:

    MyRobot
        src
            standard
            org
                first
                    ...
