## Using GitHub CodeSpaces for KCL C++ module

The codespace configuration is on the 'codespace' branch. This branch is set
up for prebuilds: each push to this branch will trigger a prebuild of the
codespace, which will speed up subsequent startup of codespaces.

Therefore, any change to the _configuration_ of the codespace should be pushed
to that branch. All other branches should then be rebased onto that branch, to
ensure they all share the same configuration, ensuring they can all be started
from the same prebuilt codespace.

The idea otherwise is to have each branch correspond to a particular task or
assignment. The `README.md` file (i.e. this file) should be updated with all
the relevant information for the task, as this will be the first file shown in
the codespace (appropriately rendered for Markdown).

Scripts and other commands can be placed in the `.bin/` folder, which is
configured to be in the `PATH` within the codespace. This can be done without
requiring an update to the `codespace` branch (though it's probably good
practice to do so if the added script is intended to be available on all
assignments).

To set up a new task or assignment, create a new branch from the `codespace`
branch, and add/modify as required. You can then push your changes to their
own branch, with a clear label to identify the assignment. This allows students
to pick the appropriate assignment from the branch drop-down selection menu,
and start their own codespace from there.
