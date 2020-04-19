# nPose-Facial-Layering-Plugin
Requires
* nPose V4.00

Click the [Releases](https://github.com/nPoseTeam/nPose-Facial-Layering-Plugin/releases) tag above for prior release version which support prior versions of nPose.

Use this plugin if Layering another animation on top of an existing pose is required. There are two types of layering animations to consider:
1. Facial animations which could include Bento joint animations.  
  This type of layering utilizes a built in looping within the scripts.  
  This type of layering is associated with a single pose in a single seat, meaning the animation will be removed when a pose is changed for this particular seat.  
  https://github.com/nPoseTeam/nPose-V4/wiki/NC-Contents#xanim
        
2. Simply called Layering animations which could include a full animation or partial animation.  
  This type of layering does not automatically loop and will only loop if the animation is uploaded to SL as a looping one. Layering can also be used for Bento animations not intended to loop.  
  This type of layering is associated with Avatar however not with any specific pose.  
    When using LINKMSG to call this function the Avatar will be the menu user.   
    When using SATMSG/NOTSATMSG to call this function the Avatar will be who is seated where the MSG is associated with.   
  This type of layering must be specifically turned off by instructions.  
  Access layering via LINKMSG or SATMSG/NOTSATMSG.  
  
  When using 'stopAll' nPose will stop all layered animations currently imposed on this Avatar.   
  When using 'stop,[animName] nPose will stop the single animation of name 'animName'.   
  When using 'start,[animName]' nPose will start the single animation of name 'animName'.  To start multiple anims, use multiple LINKMSG lines.   
  
   The syntax is as follows:   
    *  `LINKMSG|-218|%AVKEY%/stopAll`   
    *  `LINKMSG|-218|%AVKEY%/stop,[animName]`    
    *  `LINKMSG|-218|%AVKEY%/start,[animName]`     
    
    

Documentation: https://github.com/nPoseTeam/nPose-Facial-Layering-Plugin  
Support group: secondlife:///app/group/f61cb811-89c4-cec7-daa9-067b3f851f9a/about  
Headquarter/Shop: http://maps.secondlife.com/secondlife/Newt/131/197/60  
Report issues to: https://github.com/nPoseTeam/nPose-Facial-Layering-Plugin/issues  
or (if you don't have a GitHub account) send a IM to  
Howard: Howard Baxton (english)  
Leona: slmember1 Resident (german, english)
