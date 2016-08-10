# David

On the technical part I was responsible for the communication between the Myo server and the betaCube.
This included defining a protocol,
    setting up a C++-TCP-Server with an easy-to-use API to send grab and delete events,
    and setting up a C#-TCP-Client with an easy-to-use listener interface for the betaCube. 
Also, I intensively worked with Felix on trying to stabilize the offset calculation that enables us to get rid of the colored wristbands.

During field testing I was usually responsible for climbing the route over and over again
    and actively helped debugging the betaCube.

For the proposal I drafted the abstract, introduction and goals section and polished the whole thing together with my team mates.
For the final report I drafted the abstract, introduction, evaluation, conclusion and parts of the implementation section.
I also helped finalizing the report after all drafts were written.
Together with my team I helped structuring, designing and holding our presentations.

Finally, I felt responsible for basic project and team management (including setting up infrastructure, organizing meetings, etc.).
However, this was not a hard task, as in my opinion our team was working together very well.

# Marc

My main technical contribution to this project was implementing the logic into the betaCube-system. 
In particular this meant connecting to the Myo Server using the provided and easy-to-use C#-TCP-Client and interpreting the different JSON-messages.
Depending on the message then different task had to be implemented. 

In case of a grab-event, the color-search had to be queried to determine the location data of the visual markers.
This data had to be post-processed in the latest version (using markers at the Myo-wearables insead of coloring the hands), in order to compute the hand location.
Lastly using the determined hand location, the nearest hold in a t-neighborhood could be determined. 
This hold then became the new end (top-hold) of the route defined up to this point. 
In case of a deletion event the top-hold was simply removed from the route. 
Furthermore, it has to be mentioned that it was my part of my work to visualize and project the route including different hold types and other data to the climbing wall. 

While testing I monitored and debugged the betaCube together with Anna, who was responsible for the color-search. 
However, as part of a team we all worked together on designing, testing and debugging various parts of the project.

Writing the proposal I contributed to and/or wrote the related work section, the references section and the milestones section. 
For the final report I again contributed the related work section, the references section and technical concept of deleting previously grabbed holds. 
All together we finalized and polished the documents. 
I helped structuring, designing and holding our presentations together with the rest of my team.

Furthermore, I contributed to the project and team management, e.g. by organizing, structuring and setting up the templates for both the documents and presentations as discussed.

Lastly, it has to be mentioned that I sincerely enjoyed working with this team. 
Every member actively participated and contributed to the success of this project.

# Felix

My contribution to the Seminar project was basically the implementation of the Myo software.
In the first half of the seminar I implemented and tested the grab detection of the Myo based on the EMG-Data provided by the armband.
The program requests the server, that was written by David, to send a message to the betaCube when it detects a grabbed hold.
In the second half I extended the grab detection with the orientation data to compute the offset of the hand compared to the position of the armband.
So I implemented some trigonometric functionality and a distance based sampling to get correct offset from the orientation data of the Myo.
Together with David, I debugged and tested the offset computation.

While the team meetings I setted up and controlled the Myo server together with the grab detection and organized the network connection between the Myo server and the betaCube.
I also organized the spray cans and colored the sheets of paper we needed for the hands and Myos to be able to recognise them in the color detection.
Furthermore, I prepared the Myos for the team meetings.

In the final report and in the proposal I wrote some parts of the implementation section, which deal with the Myo muscle tracker and the grab detection.
In addition I helped finalizing and correcting the reports.

In the end I want to say that everybody in the team worked a lot for the project.
Therefore all team meetings were very productive and successful.

#Anna

I was responsible for image analysis part of the project.
That included image retrieval from Kinect and locating the position of hands and feet on the wall.
Hands and feet were color coded, so my task was to find the coordinates of a specific color from the image.
To make color search more light-independent, we used differences between RGB components to distinguish colors.
When color search was implemented, I was dealing with the optimization of the process.

During testing phase, I monitored and debugged the betaCube together with Marc.
Most of the time, out team was working together to test, debug and improve our project.

Together with my teammates, we wrote both proposal and final report.
All of us participaed in structuring, designing and holding our presentations.

Finally, I think that every member of the team made a great contribution to the project.
Everyone worked hard at home as well as during our meetings.
I enjoyed working with this team.
