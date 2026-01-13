- What does BPML stand for? #card
	- Business Process Modelling Language
- What information needs to be extracted from a process model? #card
	- What is to be done?
	- Who is doing it?
	- When is it supposed to be done?
	- Where is it supposed to be done?
	- Why is it done?
	- How is it executed?
	- Who is dependent on this being done?
- How do BPMLs differ to process models? #card
	- The extent to which their constructs highlight the answers to:
		- What is to be done?
		  id:: 69622ebb-9db0-4b52-8ab7-557b9e6c50cf
		- Who is doing it?
		- When is it supposed to be done?
		- Where is it supposed to be done?
		- Why is it done?
		- How is it executed?
		- Who is dependent on this being done?
- What can inform differences in BPMLs? #card
	- Source Domains
	- Targeted Applications
- What are the three purposes of a Business Process? #card
	- Description
	- Analysis
	- Enactment
- Why is modelling necessary to describe business processes? #card
	- Communicate to other people
	- Define or share it across a group of people
- Why is modelling necessary to analyse a business process? #card
	- Changing the order of activities
	- Changing responsibilities
	- Improving the process
- Why is modelling necessary to enact a business process? #card
	- The ability to transfer it to executable code
- What are BPMLs generally good at and generally bad at? #card
	- The are generally good at describing functional and behavioral perspectives
	- They tend to only partially support organisational and informational perspectives
- What role does graphical modelling play in process management projects? #card
	- They are important tools in design, re-design, enactment, and evolution of business processes.
	- They regularly consume a lot of time and resources in process management projects
- What is BPMN? #card
	- A recently published notation standard for business processes
- Who designed BPMN? #card
	- BPMI.org
	- February 2006
- What is the primary goal of BPMN? #card
	- Provide notation that is readily understandable by all business users
		- Business analysts (design the processes)
		- Technical developers (Implementing the technology to support those processes)
		- Business people (monitor and manage those processes)
	- Create a standardized bridge between process design and process implementation
	- Ensure that XML languages designed to execute business processes can be visualised
- What are the three broad types of diagrams? #card
	- Collaboration
	- Process
	- Choreography
- What is the *intent* of BPML? #card
	- Standardize business process model notation in the face of many different notations and viewpoints
	- Providing a simple means of communicating process information to other:
		- Business users
		- Process implementors
		- Customers
		- Suppliers
- Examples of other diagrams that are not BPMN (by The Object Management Group) #card
	- UML activity diagram
	- UML EDOC (Enterprise Distributed Object Computing) Business Process
	- IDEF
	- ebXML
	- BPSS
	- Activity-Action flow diagram
	- RosettaNet
	- LOVeM
	- Event process chains
- Example of an XML language designed for modelling business processes #card
	- WSBPEL (Web Services Business Protocol Execution Language)
- Seven Process modelling guidelines #card
	- Use as few elements in the model as possible.
	  logseq.order-list-type:: number
		- Why use a few elements as possible? #card
			- Larger models are more difficult to understand
			- They are more error prone
	- Minimize the routing paths **per element**
	  logseq.order-list-type:: number
		- High degree elements are more difficult to understand
	- Use only one start event and one end event
	  logseq.order-list-type:: number
		- Less error prone
		- Easier to analyse
	- Model as structured as possible
	  logseq.order-list-type:: number
		- When is a process model structured? #card
			- When every split connector matches a join connector of the same type.
			  logseq.order-list-type:: number
	- Avoid OR routing elements.
	  logseq.order-list-type:: number
		- Instead of using OR routing elements, what should you opt for? #card
			- AND or XOR
	- Use verb-object activity labels
	  logseq.order-list-type:: number
	- Decompose models with more than 50 elements
	  logseq.order-list-type:: number
- Ten anti-patterns for modelling processes: #card
	- Activities in one pool are not connected
	  logseq.order-list-type:: number
	- The event does not contain an end event
	  logseq.order-list-type:: number
	- Sequence flow crosses sub-process boundary
	  logseq.order-list-type:: number
	- Sequence flow crosses pool boundary
	  logseq.order-list-type:: number
	- Gateway receives, evaluates and sends a message
	  logseq.order-list-type:: number
	- Intermediate events are placed at the edge of a pool
	  logseq.order-list-type:: number
	- Hanging intermediate events or activities in the process model
	  logseq.order-list-type:: number
	- Each swimlane in a pool has a start event
	  logseq.order-list-type:: number
	- Exception flow not connected to the exception
	  logseq.order-list-type:: number
	- Message flow misuse across swimlanes
	  logseq.order-list-type:: number
- BPMN Rubrik #card
	- Correct symbol set
	- All sequential tasks performed by one role are grouped into one task
	- All tasks are Verb-Object formatted
	- Pools for companies/organisations (sometimes customers)
	- Each pool has a single start and single end node
	- All sequences in a pool should be connected
	- No crossing sequence or inter pool sequences
	- Each gateway has type shown and at least 3 sequence flows
		- XOR gateways have conditional expressions