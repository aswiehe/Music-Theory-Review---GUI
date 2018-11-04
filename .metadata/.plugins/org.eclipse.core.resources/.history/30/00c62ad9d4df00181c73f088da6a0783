
import java.util.ArrayList;
import java.util.Arrays;

// JavaFX Classes

import javafx.application.Application;

import javafx.stage.Stage;
import javafx.scene.Scene;

import javafx.scene.layout.Pane;
import javafx.scene.text.Text;
import javafx.scene.layout.HBox;
import javafx.scene.layout.VBox;

import javafx.geometry.Insets;

import javafx.scene.control.Button;

public class StartGUI extends Application {
  @Override // Override the start method in the Application class
  public void start(Stage primaryStage) {
    // Create a master pane
    Pane pane = new HBox(10);
    pane.setPadding(new Insets(20, 20, 20, 20));
    
    
    // Create hbox in left pane to hold vboxes with buttons
    Pane leftPane = new HBox(10);
    pane.getChildren().add(leftPane);
    
    // Create vboxes to hold buttons
    VBox noteVBox = new VBox();
    VBox accidentalVBox = new VBox();
    VBox octaveVBox = new VBox();
    
    // Set spacing for vboxes in left pane
    noteVBox.setSpacing(5);
    accidentalVBox.setSpacing(5);
    octaveVBox.setSpacing(5);
    
    // Add buttons to noteVbox
    Button cButton = new Button("C");
    Button dButton = new Button("D");
    Button eButton = new Button("E");
    Button fButton = new Button("F");
    Button gButton = new Button("G");
    Button aButton = new Button("A");
    Button bButton = new Button("B");
    Button[] noteButtons = {cButton, dButton, eButton, fButton, gButton, aButton, bButton};
    // set button width
    for(int i = 0; i < noteButtons.length; i++) {
    	noteButtons[i].setPrefWidth(80);
    }
    ArrayList<Button> noteButtonArrList = new ArrayList<>();
    noteButtonArrList.addAll(Arrays.asList(noteButtons));
    
    // Add buttons to accidentalVbox
    Button flatButton = new Button("Flat");
    Button naturalButton = new Button("Natural");
    Button sharpButton = new Button("Sharp");
    Button[] accidentalButtons = {flatButton, naturalButton, sharpButton};
    // set button width
    for(int i = 0; i < accidentalButtons.length; i++) {
    	accidentalButtons[i].setPrefWidth(80);
    }
    ArrayList<Button> accidentalButtonArrList = new ArrayList<>();
    accidentalButtonArrList.addAll(Arrays.asList(accidentalButtons));
    
    // Add buttons to octaveVbox
    Button zeroOctaveButton = new Button("Zero");
    Button firstOctaveButton = new Button("First");
    Button secondOctaveButton = new Button("Second");
    Button thirdOctaveButton = new Button("Third");
    Button fourthOctaveButton = new Button("Fourth");
    Button fifthOctaveButton = new Button("Fifth");
    Button sixthOctaveButton = new Button("Sixth");
    Button seventhOctaveButton = new Button("Seventh");
    Button eighthOctaveButton = new Button("Eighth");
    Button ninthOctaveButton = new Button("Ninth");
    Button tenthOctaveButton = new Button("Tenth");
    Button eleventhOctaveButton = new Button("Eleventh");
    Button twelfthOctaveButton = new Button("Twelfth");
    Button[] octaveButtons = {zeroOctaveButton, firstOctaveButton, secondOctaveButton, thirdOctaveButton, fourthOctaveButton, fifthOctaveButton, sixthOctaveButton, seventhOctaveButton, eighthOctaveButton, ninthOctaveButton, tenthOctaveButton, eleventhOctaveButton, twelfthOctaveButton};
    // set button width
    for(int i = 0; i < octaveButtons.length; i++) {
    	octaveButtons[i].setPrefWidth(80);
    }
    ArrayList<Button> octaveButtonArrList = new ArrayList<>();
    octaveButtonArrList.addAll(Arrays.asList(octaveButtons));
    
    // Add vbox buttons to their respective vboxes in leftpane
    noteVBox.getChildren().addAll(noteButtonArrList);
    accidentalVBox.getChildren().addAll(accidentalButtonArrList);
    octaveVBox.getChildren().addAll(octaveButtonArrList);
    Pane[] pitchPropertyVBoxes = {noteVBox, accidentalVBox, octaveVBox};
    ArrayList<Pane> pitchPropertyVBoxArrList = new ArrayList<>();
    pitchPropertyVBoxArrList.addAll(Arrays.asList(pitchPropertyVBoxes));
    
    // Add pitch property vboxes holding buttons to leftpane
    leftPane.getChildren().addAll(pitchPropertyVBoxArrList);
    
    // Create pane in right pane to hold text to show the pitch selected/built
    Pane rightPane = new Pane();
    Text rightPaneText = new Text("right pane text (to show something like C - Natural (Eighth Octave)");
    rightPane.getChildren().add(rightPaneText);
    pane.getChildren().add(rightPane);
        
    // Create a scene and place it in the stage
    Scene scene = new Scene(pane);
    // Set the title
    primaryStage.setTitle("Music Theory Review - GUI");
    // set the scene for the stage
    primaryStage.setScene(scene);
    // show the stage
    primaryStage.show();
  }

  public static void main(String[] args) {
    launch(args);
  }
}