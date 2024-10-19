import java.util.Scanner;

class Project {
    private String name;
    private int votes;

    public Project(String name) {
        this.name = name;
        this.votes = 0;
    }

    public String getName() {
        return name;
    }

    public int getVotes() {
        return votes;
    }

    public void addVote() {
        votes++;
    }

 
    public String toString() {
        return name + " has " + votes + " vote(s)";
    }
}


class VotingSystem {
    private ArrayList<Project> projects;

    public VotingSystem() {
        projects = new ArrayList<>();
    }

    public void addProject(String projectName) {
        projects.add(new Project(projectName));
    }
