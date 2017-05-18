 <link rel="stylesheet" href="{{baseUrl}}/book/requirements/useCases/css/useCases.css">

The Main Success Scenario (MSS) describes the most straightforward interaction for a given use case, which assumes that nothing goes wrong. This is also called the _Basic Course of Action_ or the _Main Flow of Events_ of a use case. Given below is another example of an MSS.

<tip-box>
	<div>
		<ul>
			<li>System: Online Banking System (OBS)</li>
			<li> Use case: UC23 - Transfer Money </li>
			<li> Actor: User </li>
			<li> MSS:
				<ol>
					<li>User chooses to transfer money.</li>
					<li>OBS requests for details of the transfer.</li>
					<li>User enters the requested details.</li>
					<li>OBS requests for confirmation.</li>
					<li>OBS transfers the money and displays the new account balance.</li>
					<li class="custom-bullet-point">Use case ends.</li>
				</ol>
			</li>
			<li> Extensions:
				<ol>
					<li class="custom-bullet-point">3a. OBS detects an error in the entered data.
						<ol>
							<li class="custom-bullet-point">3a1. OBS requests for the correct data.</li>
							<li class="custom-bullet-point">3a2. User enters new data.</li>
							<li class="custom-bullet-point ">Steps 3a1-3a2 are repeated until the data entered are correct.</li>
							<li class="custom-bullet-point ">Use case resumes from step 4.</li>
						</ol>
					</li>
					<li class="custom-bullet-point">3b. User requests to effect the transfer in a future date.
						<ol>
							<li class="custom-bullet-point">3b1. OBS requests for confirmation.</li>
							<li class="custom-bullet-point">3b2. User confirms future transfer.</li>
							<li class="custom-bullet-point">Use case ends.</li>
						</ol>
					</li>
					<li class="custom-bullet-point">*a. At any time, User chooses to cancel the transfer.
						<ol>
							<li class="custom-bullet-point">*a1. OBS requests to confirm the cancellation.</li>
							<li class="custom-bullet-point">*a2. User confirms the cancellation.</li>
							<li class="custom-bullet-point">Use case ends.</li>
						</ol>
					</li>
					<li class="custom-bullet-point">*b. At any time, 120 seconds lapse without any input from the User.
						<ol>
							<li class="custom-bullet-point">*b1. OBS cancels the transfer.</li>
							<li class="custom-bullet-point">*b2. OBS informs the User of the cancellation.</li>
							<li class="custom-bullet-point">Use case ends.</li>
						</ol>
					</li>
				</ol>
			</li>
		</ul>
	</div>

Note how the MSS assumes that all entered details are correct and ignores problems such as timeouts, network outages etc. MSS does not tell us what happens if the user enters incorrect data.

</tip-box>
