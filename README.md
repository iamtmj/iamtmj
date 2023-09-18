package main

import (
	"fmt"
)

type Bio map[string]string

func main() {
	for k, v := range GetBio() {
		fmt.Printf("%+v: %+v\n", k, v)
	}
}

func GetBio() Bio {
	return Bio{
		"- ⚡ Quick bio:":                    "Manan here, a coding enthusiast who embraces math and enjoys the beauty of music.",
		"- 🔭 I’m currently working on":      "The Logic Workshop,Mirine Studios",
		"- 🌱 Skills":        "Game Development,3D Modeling,Algorithm Design",
		"- 📫 How to reach me:":              "officialmananjindal@gmail.com",
	}
}
