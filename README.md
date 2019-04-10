# CenterSeekbar
Custom seekbar that start from the center 

![](slider.gif)

public class MainActivity extends AppCompatActivity {

    private CenterPointSeekBar seekBar;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        seekBar=findViewById(R.id.seekbar);
        seekBar.setProgress(3);
        seekBar.setOnSeekBarChangeListener(new CenterPointSeekBar.OnSeekBarChangeListener() {
            @Override
            public void onOnSeekBarValueChange(CenterPointSeekBar bar, double value) {

            }
        });

    }
}


Step 1. Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
Step 2. Add the dependency

	dependencies {
	        implementation 'com.github.atiqulalam:CenterSeekbar:1.0.0'
	}

