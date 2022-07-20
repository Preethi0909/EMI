package com.emi;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;

public class home extends AppCompatActivity implements View.OnClickListener {
    Button b1;
    EditText et1,et2,et3,et4;
    TextView txt;


    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_home);

        b1=(Button)findViewById(R.id.homebtn);
        b1.setOnClickListener(this);
        et1=(EditText)findViewById(R.id.homepa);
        et2=(EditText)findViewById(R.id.homedp);
        et3=(EditText)findViewById(R.id.homeir);
        et4=(EditText)findViewById(R.id.homeit);
        txt=(TextView)findViewById(R.id.homeemi);
        Intent intent=getIntent();

    }

    public void onClick(View view) {
        double p,r,n,d,emi;
        p=Double.parseDouble(et1.getText().toString());
        d=Double.parseDouble(et2.getText().toString());
        p=p-d;
        r=Double.parseDouble(et3.getText().toString());
        r=r/(12*100);
        n=Double.parseDouble(et4.getText().toString());

        emi=p*(r*Math.pow((1+r),n))/(Math.pow((1+r),n)-1);
        emi=emi/12;

        txt.setText(String.valueOf(emi));

    }
}
