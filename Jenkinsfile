#!/usr/bin/env groovy
//Leave the above line alone.  It identifies this as a groovy script.
@Library('dcaf-scripts@diff-timeout')
//Modify the below parameters to match the values for this particular repo

def utfPaths = ["source\\FPGA Module.lvproj"]
def vipbPaths = ["source\\DCAF FPGA.vipb"]
def lvVersion = "14.0"

node("proto")
{
	//Leave the below line alone.  It pulls in the pipeline definition from the DCAF buildsystem repo so we don't duplicate code in every repo 
	dcafPipeline(utfPaths,vipbPaths,lvVersion)
}