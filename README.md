# android-dial-picker
A custom circular rotating dial like picker for android.  

## Implementation

Android Dial Picker, a circular custom view that works just like a rotating dial. The dial can be customized according to the needs of the 
user like the direction(left,top,right,bottom), max/min ranges, interval values and colours. These custom attributes can be added and styled via XML as well as programatically.  
As the dial rotates, the current value gets updated and is displayed on the screen.  

![Alt Text](https://github.com/moldedbits/android-dial-picker/blob/master/gif/dial.gif)

## Usage
* In XML layout:
```
<com.moldedbits.dialpicker.DialView
        android:id="@+id/dial_left"
        android:layout_width="90dp"
        android:layout_height="200dp"
        android:layout_alignParentStart="true"
        android:layout_centerInParent="true"
        android:layout_marginTop="@dimen/margin_normal"
        android:padding="5dp"
        custom:centerPadding="50"
        custom:dialDirection="LEFT"
        custom:endColor="#FF8A80"
        custom:intervalValueOnLine="true"
        custom:leastCount="1"
        custom:lineInterval="2"
        custom:maxValue="24"
        custom:minValue="0"
        custom:paintArcColor="@color/smoke_red"
        custom:paintLineColor="@color/smoke_red"
        custom:paintTextColor="@color/smoke_red"
        custom:startColor="#FF8A80"
        custom:textSize="14"
        custom:tickGapAngle="12" />
```
* All customizable attributes: In attrs.xml 
```
<declare-styleable name="DialView">
        <attr name="lineInterval" format="integer" />
        <attr name="maxValue" format="integer" />
        <attr name="minValue" format="integer" />
        <attr name="centerPadding" format="integer" />
        <attr name="leastCount" format="integer" />
        <attr name="tickGapAngle" format="integer" />
        <attr name="textSize" format="integer" />
        <attr name="intervalValueOnLine" format="boolean" />

        <attr name="dialDirection" format="enum">
            <enum name="LEFT" value="1" />
            <enum name="TOP" value="2" />
            <enum name="RIGHT" value="3" />
            <enum name="BOTTOM" value="4" />
        </attr>
        <attr name="startColor" format="color"/>
        <attr name="endColor" format="color"/>
        <attr name="paintLineColor" format="color"/>
        <attr name="paintTextColor" format="color"/>
        <attr name="paintArcColor" format="color"/>
    </declare-styleable>
```
Please feel to contribute or report issues.

