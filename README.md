# comp304-project-2--electronic-voting-system-solved
**TO GET THIS SOLUTION VISIT:** [COMP304 Project 2 -Electronic Voting System Solved](https://www.ankitcodinghub.com/product/comp-304-project-2-electronic-voting-system-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117708&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP304 Project 2 -Electronic Voting System Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Electronic Voting Simulation

The Republic of Banana is planning to upgrade its voting process by introducing electronic voting stations for the upcoming presidential election. However, the election committee intends to test the new electronic voting system with a simulator before implementing it in the actual elections.

Your task in this project is to develop a simulator that can replicate an election day scenario. The simulator should include the modeling of independent voters waiting in queues to cast their votes, polling stations for voting, and regular maintenance in case of any failures. It is crucial to ensure that the simulation is race-free and deadlock-free to prevent any miscounts or disruptions during the voting process.

In this project, you are required to use the POSIX threads (pthreads) API to implement the simulation. You will get more familiar with the concepts of scheduling, synchronisation, multi-threading and deadlock prevention in operating systems.

Simulation Settings

Each voter will be voting at a single polling station and will cast their vote to one for the presidential candidate. The presidential candidates are Mary, John, and Anna, with 40%, 15%, and 45% chances of getting elected, respectively.

To simulate the election day scenario, there are four parts that need to be implemented, each building upon the previous one in increasing complexity. It is recommended to implement the simulation parts in order, starting from Part 1 and moving towards Part 4. This way, you can build upon each previous part’s functionality and ensure that the entire simulation is working correctly.

1

Part I ELECTRONIC VOTING SIMULATION

Part I

(40 points) When a voter arrives at the polling station, they will need to click on the queue machine to get their position number in the queue. A separate screen will display the next voter (signals/wakes up) who should go to the polling station. Once their turn comes, the voter will go to the polling station and cast their votes for the presidential candidate of their choice. Here are more detailed rules for the simulation environment.

• The simulation should use real-time. Get the current time of the day, run the simulation until current time + simulation time.

• There is a single polling station that is used.

• There is only one voter using the polling station at any time.

• A new voter arrives to the polling station with probability p at every t secs and uses the queuing machine to get their position on the queue.

• Each voter takes 2t secs to cast their vote (sleep the thread for 2t secs). • The vote can be to any of the aforementioned candidates, with the following probabilities (Mary: 40, John: 15, Anna: 45)

• After a voter finishes voting, they have no consequence on the simulation.

• It is not allowed for a voter to use the polling station without their queue number being shown on the display (a voter cannot acquire a lock from another voter to access the polling station).

• Use command line arguments -t and -p to indicate the total simulation time (e.g. -t 200) and probability (e.g. 0.5), respectively.

In real life, t is usually in the order of minutes but assume t is 1 sec for the purpose of the computer simulation.

Part II

(30 points) In this section, we will add a priority system for certain voters. The queuing machine favors the elderly and pregnant women voters (assume that the voter enters their national identity number to get a queuing position). Now in addition to creating a voter with probability p at every t, create a pregnant/elderly voter with probability 1-p at every t. The queuing machine must favor elderly or pregnant women and let them vote until one of following conditions hold:

• (a) No more elderly or pregnant women are waiting,

• (b) 5 or more non-elderly non-pregnant voters are lined up to vote.

Part III KEEPING LOGS

Note that this solution now causes starvation to the elderly and pregnant voters. Suggest and implement a solution to avoid starvation of the elderly and pregnant voters. Briefly explain why starvation for the elderly and pregnant voters occurs and how you solve it in your report. You can play with p to enforce starvation to test your solution.

Part III

Part IV

(20 points) Now instead of having a single polling station, there will be multiple polling stations. Each polling station will have its own queuing machine. Make sure the voting counters for each polling station are independent. Whenever a new voter arrives, assign him/her to the polling station which is least busy. Busyness here is evaluated based on the number of people waiting to cast their votes. Each of the new polling stations can still fail the same way noted in part III, and the polling machine’s respective voters will have to wait. Make -c as a command line argument to specify the number of polling stations in the simulation.

Keeping Logs

(10 points) You are required to keep a log for the voters and for the queuing machine, which will help you debug and test your code. The voters.log should keep the station ID, voters ID, their category (special (S) or ordinary (O) or mechanic (M)), the request time the voters requested their queue position, the polling station time (end of polling station usage), turnaround time (polling station time – request time).

StationID.VoterID Category Request Time Polling Station Time Turnaround Time

1.1 S 0 2 2

1.2 O 0 4 4

Output the snapshot of the waiting voters with their IDs and categories, in addition to the current votes, in every second starting from nth secs to the terminal, where n is also a command line argument. The numbers indicates the voter IDs waiting in the queue at time n.

Feel free to come up with a better representation or GUI.

DELIVERABLES Example output:

At 20 sec, polling station 1, elderly/pregnant: 16, 18, 20

At 20 sec, polling station 1, ordinary : 23, 25

At 20 sec, polling station 2, elderly/pregnant: 17, 19

At 20 sec, polling station 2, ordinary : 21, 24, 26

At 20 sec total votes: (Mary: 4, John: 2, Anna: 3)

…

Also to initialize the queuing simulation, make sure the following is done: • At time zero, there is one none-elderly none-pregnant woman voter waiting to vote and one elderly or pregnant woman waiting to vote. (in total 2 waiting)

Implementation

• You should represent each voter as a thread. The queuing machine should have its own separate thread.

• Start simple. For example simulate Part 1 and make sure it works correctly. Add complexity as you move to the other parts.

• To sleep pthreads, please use the code that we provided on blackboard. Do not use sleep() system call.

• For Pthread semaphores, mutexes and condition variables, also refer to the pthread tutorial online: https://hpc-tutorials.llnl.gov/posix/

Deliverables

You are required to submit the followings packed in a zip file (named your-username(s).zip) to blackboard :

• .c or .cpp source file that implements the simulation. Please comment your implementation.

• sample log files for 60 sec simulation for p=0.5.

DELIVERABLES • any supplementary files for your implementation (e.g. Makefile)

• a README (report) file describing your implementation, particularly which parts of your code work. Since we cannot hold a demo with everyone, document your report properly.

• We will share the github classroom link soon.

GOOD LUCK.
