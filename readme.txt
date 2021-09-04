Hey!

Here I am updating files/steps to configure CICD to your projects using Gitlab-Runner.
(We are doing the below steps in a windows VM)
First you need to configure and register your gitlab runner and then paste the respective gitlab-ci.yml file along with the repo at the root position.

You can configure/register your gitlab runner by following the below steps or by following the link below:
Link: youtube.com/watch?v=2MBhxk2chhM

1. Login to your VM
2. Download the respective gitlab runner that suits your VM/system
3. Paste the .exe file inside local disk C
4. Name the above folder as Gitlab-Runner
5. Also rename the .exe file to gitlab-runner.exe
6. Type cmd in the search in taskbar
7. Open the command prompt in adminstrator mode
8. Copy the location of the .exe file mentioned above and paste the following command in the cmd prompt-
   cd C:\Gitlab-Runner
9. Now type the following command:
   gitlab-runner.exe register

##############################################################################
##############################################################################
The below details can be obtained (if you have access/permissions of the repo)
Click on Settings in the left sidebar
Opt for CICD inside Settings
Opt the 2nd option (Runner commands)
Expand the above runner Settings
Below you can see the branch link and tokens
Active runners can be seen below.
##############################################################################
##############################################################################

10. Type the gitlab branch link from your respective gitlab repo
11. Type the token of your respective gitlab branch from the repo
12. Give a name to your gitlab runner (You can give 'project-name-runner)
13. Give tag names as needed.
14. Give executor as shell
15. Your gitlab runner has been registered successfully.

Now rename the yml file(remove project code format from the starting of yml files attached) to gitlab-ci.yml
Paste the renamed yml file inside the repo root location.

Hope this helps, as I found it really hard to get resources to do the above in a windows VM.

Thank You!