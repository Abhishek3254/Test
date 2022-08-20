# Test
public class Planet {
	String nameOfPlanet[]={"Mercury","Venus","Earth","Jupitor","Saturn","Uranus"};
	String surfGases[]={"Carbon Dioxide","Nitrogen","Oxygen","Hydrogen","Helium","Methane"};
	int NoOfMoons[]={0,0,1,79,83,27};
	String rings[]={"NO","NO","NO","YES","YES","YES"};
	public int countMoon(){
		int c=0;
		for(int i=0;i<rings.length;i++){
			if(rings[i]=="YES")
				c=c+NoOfMoons[i];
		}
		return c;
	}
	public String toString(){	
		return surfGases[3]+" "+surfGases[4];
	}
	public static void main(String[] args) {
		 Planet p=new  Planet();
		 System.out.println(p.countMoon());
	        System.out.println(p);
		
	}
}
