# CenterSeekbar
Custom seekbar that start from the center 

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
