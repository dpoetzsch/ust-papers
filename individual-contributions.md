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
