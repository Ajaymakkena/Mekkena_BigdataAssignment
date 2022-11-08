https://beam.apache.org/get-started/quickstart-java/

mvn archetype:generate `
  -D archetypeGroupId=org.apache.beam `
  -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
  -D archetypeVersion=2.42.0 `
  -D groupId=org.example `
  -D artifactId=word-count-beam `
  -D version="0.1" `
  -D package=org.apache.beam.examples `
  -D interactiveMode=false
   
cd .\word-count-beam

dir .\src\main\java\org\apache\beam\examples

In the word-count-beam directory, create a file called sample.txt. Add some text to the file. For this example

mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner

ls counts*
   
more counts*

Output :

borne: 1
When: 3
ugly: 1
tongue: 1
tune: 1
keeps: 1
distracted: 1
help: 1
great: 2
kind: 1
believed: 1
patient: 1
shut: 1
country: 1
round: 1
Thus: 2
demands: 1
can: 2
O: 7
their: 4
much: 3
returns: 1
come: 1
humbly: 1
yours: 1
You: 2
days: 1
thank: 1
court: 1
hold: 1
helps: 1
plague: 1
die: 2
need: 1
sweet: 3
amble: 1
grief: 2
gifts: 1
these: 3
Shakespeare: 2
slings: 1
gather: 1
With: 5
circumstance: 1
go: 4
awry: 1
loneliness: 1
turn: 1
Exit: 2
lawful: 1
rich: 1
frankly: 1
hue: 1
act: 1
-- More  --

