# maudSoliditySmartContract
Voting system smart contract


Je n'ai pas pu initier le event workflowstatusChange.
Je voulais le faire en utilisant le contructeur de cette manière:


construtor(){
Workflowstatus = RegisteringVoters;
}

  event WorkflowStatusChange(WorkflowStatus previousStatus, WorkflowStatus newStatus);

et dans mais fonctions de changement (en updatant respectivement chaque status comme suite):


 function startingRegistration() onlyOwner public {
        WorkflowStatus = ProposalsRegistrationStarted;
       emit WorkflowStatusChange(WorkflowStatus.RegisteringVoters, WorkflowStatus);
   }
   
   
 Mais cela revenait avec une erreur :( 
   
