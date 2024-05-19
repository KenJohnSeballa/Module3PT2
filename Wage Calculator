import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {
    EditText hoursWorkedInput, hourlyRateInput;
    TextView resultText;
    Button calculateButton;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        hoursWorkedInput = findViewById(R.id.hoursWorkedInput);
        hourlyRateInput = findViewById(R.id.hourlyRateInput);
        resultText = findViewById(R.id.resultText);
        calculateButton = findViewById(R.id.calculateButton);

        calculateButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                calculateWage();
            }
        });
    }

    private void calculateWage() {
        double hoursWorked = Double.parseDouble(hoursWorkedInput.getText().toString());
        double hourlyRate = Double.parseDouble(hourlyRateInput.getText().toString());

        double totalWage = hoursWorked * hourlyRate;

        resultText.setText("Total Wage: PHP " + totalWage);
    }
}
