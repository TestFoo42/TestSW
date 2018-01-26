**Checkout a new feature/bug-fix branch.**

		git checkout -b <branchname>
		
**Make Changes.**

		git add
		git commit -a
		
**Sync with remote to get changes you’ve missed.**

		git checkout develop
		git pull
		
**Update your feature branch with latest changes from develop by interactive rebase.**

		git checkout <branchname>
		git rebase -i --autosquash develop
		
**If you don’t have conflicts, skip this step. If you have conflicts, resolve them and continue rebase.**

		git add <file1> <file2> ...
		git rebase --continue
		
**Push your branch. Rebase will change history, so you'll have to use -f to force changes into the remote branch.**

		git push -f