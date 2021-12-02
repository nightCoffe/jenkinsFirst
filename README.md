# JenkinsFirst
plugins {
id 'java-library'
}

repositories {
mavenCentral()
}

dependencies {
testImplementation (
"com.codeborne:selenide:5.19.0",
"org.junit.jupiter:junit-jupiter-api:5.7.1",
"org.slf4j:slf4j-api:1.7.30",
"org.slf4j:slf4j-simple:1.7.30"
)
testRuntimeOnly "org.junit.jupiter:junit-jupiter-engine:5.7.1"
}

test {
useJUnitPlatform()
}