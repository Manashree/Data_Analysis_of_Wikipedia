# assignments
Template for Assignments

## Checkout an assignment

Note, **Replace** $IU_USERNAME and $HW with real values
:

	git clone git@github.iu.edu:bdossp-sp16/$IU_USERNAME.git
	cd $IU_USERNAME
	git branch $HW
	git checkout $HW
	git pull git@github.iu.edu:bdossp-sp16/assignments.git $HW
	git push -u origin $HW

For example, hw3 with 'albert' IU Username:

	git clone git@github.iu.edu:bdossp-sp16/albert.git
	cd albert
	git branch hw3
	git checkout hw3
	git pull git@github.iu.edu:bdossp-sp16/assignments.git hw3
	git push -u origin hw3


