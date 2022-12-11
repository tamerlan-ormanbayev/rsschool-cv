# Tamerlan Ormanbayev
## Contact Info
* [Github](https://github.com/timopix)
* Phone: +1(825)735-5916
* E-mail: teemopix@gmail.com
* Discord: `Timopix#7590

## About me
My name is Tamerlan Ormanbayev, I am 19 years of age, originally from Almaty, Kazakhstan. I came to Calgary, Alberta, Canada, to study the undegraduate program of Computer Science at University of Calgary. I have amazing and unique problem-solving skills, along with the burning desire to learn coding. I find a lot of tech-related things fascinating, only making me want to learn more.

## Skills
* Java
* HTML/CSS
* UX/UI
* Python
* Git

## Code examples
```
public void initialize() {

listOfFiles = folder.listFiles();
for (File listOfFile : listOfFiles) {
Files.getItems().addAll(listOfFile.getName()); //.substring(0, listOfFile.getName().indexOf(MainController.currency.toString()))); // adds a file name to listview by looping through all the files in listOfFiles
IDArray.add(Integer.parseInt(listOfFile.getName().substring(listOfFile.getName().indexOf(MainController.currency.toString())+1).replace(MainController.currency.toString(), "").replace(".csv", "")));
}
Files.getItems().clear();
for (File listOfFile : listOfFiles) {
Files.getItems().addAll(listOfFile.getName().substring(0, listOfFile.getName().indexOf(MainController.currency.toString()))); // adds a file name to listview by looping through all the files in listOfFiles
}
Files.getSelectionModel().selectedItemProperty().addListener((observableValue, s, t1) -> { //adds a listener that is keeping track of if something in a list was selected
String wallet;
currentTransaction = Files.getSelectionModel().getSelectedItem();

for (int n = 0; n < listOfFiles.length; n++) { // as long as the chosen option is in the bounds of our list of file names
if (NewId == 0) {
if (listOfFiles[n].getPath().equals("data" + File.separator + currentTransaction + MainController.currency + IDArray.get(n) + ".csv")) {// if the chosen option is inside our list XOR new file name is in currentTransaction

MainController.id = IDArray.get(n).toString();
SelectedFile = listOfFiles[n];
wallet = "data" + File.separator + currentTransaction + MainController.currency + IDArray.get(n) + ".csv";
try {
Scanner filescanner = new Scanner(new FileInputStream(wallet));
MainController.TransactionsData = CSVReader.CSV(wallet, filescanner);
switchtosceneMain();
} catch (FileNotFoundException e) {
e.printStackTrace();
} catch (IOException e) {
e.printStackTrace();
}

}
} else {
if (WalletController.rename.getPath().equals("data" + File.separator
+ currentTransaction + MainController.currency.toString() + NewId + ".csv")) {
MainController.id = String.valueOf(NewId);
SelectedFile = listOfFiles[n];
wallet = "data" + File.separator + currentTransaction + MainController.currency + NewId + ".csv";
try {
Scanner filescanner = new Scanner(new FileInputStream(wallet));
MainController.TransactionsData = CSVReader.CSV(wallet, filescanner);
switchtosceneMain();
} catch (FileNotFoundException e) {
e.printStackTrace();
} catch (IOException e) {
e.printStackTrace();
}
}
}
}
IDArray.clear();
});
}

```

## Experience
--

## Education
* BSc Undergraduate, University of Calgary, Calgary, Alberta, Canada
- Computer Science
* Harvard CS50 Online course
- Basic knowledge of Python and programming
* MIPT, Russia
- ZFTSH graduate with 3.8 GPA
* freecodecamp.org
- Responsive web design; HTML/CSS
* Codecademy
- Advanced JavaFX applications

## Languages
* English (fluent) // IELTS 8.0 (C2 level)
* Russian (native)
* Kazakh (advanced)
* German (basic)
