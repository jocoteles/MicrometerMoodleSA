**MicrometerMoodleSA** - Moodle Short Answers question generator for Micrometer
==============

This is a Moodle Short Answer question generator with the objective of teaching and evaluating the learning of the Micrometer measurement instrument. The question generator consists of a [configuration page](https://jocoteles.github.io/MicrometerMoodleSA/) that allows you to create a bank of random questions that are exported to a single file in Moodle XML format. This file can be uploaded into a Moodle course and incorporated into a Quiz Activity as a random question. Each question corresponds to a type of micrometer drawn at random and with a random opening. Configuration items are as follows:

- *Question text*. Text that will accompany the image of the micrometer drawn in the question. This text is identical for all drawn questions.
- *Types of micrometer to be included in the questions*. Allows you to choose which types of micrometers to be included in the drawing of questions (Thibles with 5, 25 and 50 divisions).
- *Thimble opacity*. Lets you choose the thimble's opacity, which in turn changes the linear scale visibility.
- *Number of random questions*. The number of random questions to include in the Moodle XML file. A high number is indicated for different students to receive different questions or for the same student to have a reduced chance of receiving a repeated question in a Quiz Activity with multiple micrometer questions.
- *Decimal separators accepted*. The type of decimal separator accepted in the student's answer can be chosen as dot and/or comma. This option is associated with the regulation of each country and the teacher's choice to make this regulation more flexible or not in the response.
- *Penalty for each wrong attempt*. Penalty for each attempt to answer the randomly selected question, ranging from 0 to 1, where 1 corresponds to 100% of the value of the question. That is, when the student makes a mistake and tries to answer it again, the value of the question is subtracted by this penalty.
- *Generate Moodle XML file*. By clicking on this button, the Moodle XML file is generated and a window for saving the file on the computer is opened to the user.
- *Render a new sample*. Button used to render the image of a micrometer sample according to the chosen settings. When clicking this button, in addition to the image of a new micrometer sample, the value of the corresponding expected reading is also shown. This sample is only intended to provide an example of the type of micrometer that will be included in the Moodle XML file.

After saving the Moodle XML file on the computer, the teacher (or course manager) must log in to the corresponding Moodle course and access the Question Bank available in Course Administration. There, a category of questions must be created that will receive the questions from the micrometer. Then, import it to the created category by selecting the option for *Moodle XML file format* and uploading the file saved on the computer. With this, the questions can be used in a Quiz Activity by adding a random question chosen from the created category.

The micrometer is shown in two distinct views. The linear scale viewing direction is perpendicular to the micrometer screw axis (reproducing the actual view during instrument reading). However, the direction of the thimble scale view corresponds to the direction of the screw axis. This choice has the didactic advantage of observing the thimble scale as a whole, facilitating the evaluation of the number of divisions for measuring the precision and reading of the instrument.

This project uses the Javascript libraries [canvg](https://github.com/canvg/canvg) and [FileSaver.js](https://github.com/eligrey/FileSaver.js/).

