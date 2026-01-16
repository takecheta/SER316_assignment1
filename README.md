git branch structure:

main ->dev ->feature2 \
main ->feature1 \
main ->feature3 \
main ->hotfix

branch description:\
main  
implements the number guessing game\

dev  
adds encouraging message to players at the start and during gameplay\

feature1  
adds quit feature\
adds ability to replay game\
improves feedback for player's guess\
adds comment documenting quit feature\

feature2\
adds variables for max attempts and game-over state\
implements logic for max attempts abd condition for game-over\

feature3\
starts hint feature\
completes hint feature\
adds hint feature to guess method\
completes test methods\

hotfix\
fixes randomInt method to include the max value

learning summary:

While merge and rebase are very similar, the way the history preserved between files differs slightly. \
Rebase takes the history between files and "combines" them to form a more linear descriptions of commits.\
Merge commit history is parallel between files thus keeping the histories "separate".\
Squash merges items, such as commits, into one. This allows cleanup of commit history when several commits fall within the same changes.\
Cherry-pick is an efficient way to merge two branches when one has a specific file to be used.\
For example, the hotfix branch only contained a change to one method, this would normally cause a merge conflict but using cherry-pick allows the method in the hotfix branch to be chosen.

feature1's git history was easy to follow but could use better organization, for instance, documenting the quit feature should have been done when the feature was implemented.

feature2's history was clean, informative, and logical.

feature3's history was confusing to follow and caused frustration when attempting to locate changes.

When working with a large team, feature2's approach seems most reasonable. Minimal commit history that also includes detailed information to identify the changes in the code.\
For smaller teams, feature3 is an understandable approach. Regular changes to the code, adding forgotten comments, implementing multiple things all make sense using feature3 and even feature2's strategies.\
A solo project with a well documented outline may suit feature1's strategy, but the lack of information shared in commit history and disorganization in implementation could cause problems even for a solo developer.

            
