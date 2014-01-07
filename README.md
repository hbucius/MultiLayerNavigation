MultiLayerNavigation
====================
#######
some Modification with the MultiLayerNavigation Project!

now I made some modify to this project , you do not need to call the method previous version,you only nedd to do:

1,if  you use system navitation return (just you don't set the return barbutton item),you don't need to do anything;

2,if  you set a custom barbuttonitem to this navigation  you need add a target to the button with the system method
  
    
    - (void) popFront:(id)sender {
    
    /*This param tell the navitation transation has animation or not! Default is YES!*/
   
    ((MLNavigationController *)self.navigationController).returnHasAnimation = NO;

    [self.navigationController popViewControllerAnimated:YES];
   
    }


 and the parameter "returnHasAnimation" decide the view transation has animation or not! Default is YES!

