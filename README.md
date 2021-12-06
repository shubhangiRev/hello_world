package com;

import java.util.ArrayList;
import java.util.Arrays;
import java.util.Iterator;
import java.util.List;
import java.util.stream.Collectors;

public class CommonElement {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		String[] gaikar = { "Shubhangi", "Parth", "Revnath", "Gaikar" };
		String[] ghule = { "Ram", "Sumati", "Shubhangi", "Parth", "Ghule" };
		List<String> gaikarlist = Arrays.asList(gaikar);
		List<String> ghulelist = Arrays.asList(ghule);
		List commonlist = gaikarlist.stream().filter(ghulelist::contains).collect(Collectors.toList());
		System.out.println(commonlist);
		
	
			
		}

	}


