## CA 125 concentration profile in 3 years

CA125 is glycoprotein usually not produced by healthy colon cells. With Vd=5l, half-time=52d,clearance 2.2ml/h, healthy concentration under 35ng/l

<bdl-fmi id="idfmi" mode="oneshot" src="CA125_healthy_tumor2.js" fminame="CA125_healthy_tumor2" tolerance="0.0000001" starttime="0" stoptime="96805000" fstepsize="500000" fpslimit="60" guid="{181fae93-2a4d-4016-8ddc-da4fd4c0a25b}" valuereferences="3,30,26" valuelabels="central.C,Cmax,tumorCellDynamicsE.y" inputs="growth,42,1,10000000,f;tumorprod,43,1,1000000000000000,f" inputlabels="tumorCellDynamicsE.g,tumorCellProduction.production"></bdl-fmi>



<bdl-chartjs-time width="800" height="300" fromid="idfmi" labels="CA125, CA125 limit" initialdata="" refindex="0" refvalues="2" maxdata="8192"></bdl-chartjs-time>

## tumor growth during 3 years, maximum growth between month 12-24 

&nbsp;&nbsp;<bdl-chartjs-time width="790" height="150" fromid="idfmi" labels="tumor size" initialdata="" refindex="2" refvalues="1" maxdata="8192"></bdl-chartjs-time>

<bdl-range id="growth" title="growth factor" min="0.1" max="10" default="3" step="0.1"></bdl-range>
<bdl-range id="tumorprod" title="tumor CA125 production" min="1" max="100" default="16" step="1">[10pg/s]</bdl-range>
