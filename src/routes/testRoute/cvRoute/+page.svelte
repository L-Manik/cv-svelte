<script lang="ts">
    import Icon from "svelte-awesome";
    import book from 'svelte-awesome/icons/book';
    import user from 'svelte-awesome/icons/user';
    import briefcase from 'svelte-awesome/icons/briefcase';
    import cogs from 'svelte-awesome/icons/cogs';

    import Section from '$components/Section.svelte'
</script>

<div class="readable-area">
    <a class="header" href="./photo.html">
        <div class="header-text">
            <h1>Squarepants, Spongebob</h1>
            <p>Menace to Society</p>
        </div>
        <img 
        class="avatar" 
        src="https://i.imgflip.com/5vwbg4.jpg" 
        alt="avatar">
    </a>

    <div class="content">
        <div class="content-column">
            <Section iconData={user} title="Profile">
                <p><b>NIK</b>: 6527469015797316<br>
                    <b>Jenis Kelamin</b>: Sponge<br>
                    <b>Tempat/Tanggal Lahir</b>: Bandung, 21 September 2001<br>
                    <b>Alamat</b>: Di dasar laut<br>
                    <b>Agama</b>: Kristen<br>
                    <b>Pekerjaan</b>: Pengangguran<br>
                    <b>Status Perkawinan</b>: Belum Kawin<br>
                </p>
            </Section>
            <Section iconData={book} title="Education">
            <ul>
                <li>
                    2011-2014
                    <br>
                    &emsp; Bikini Bottom High School
                </li>
                <li>
                    2014-2018
                    <br>
                    &emsp; New Kelp City Culinary College
                </li>
            </ul>
            </Section>
        </div>
        <div class="content-column">
            <Section iconData={briefcase} title="Work History">
            <ul>
                <li>
                    Head Cook (2022 - ongoing)
                    <br>
                    &emsp; Walter White Labs, Inc.
                </li>
                <li>
                    Marketing Associate (2020 - 2022)
                    <br>
                    &emsp; Hamlin Hamlin McGill Ltd.
                </li>
                <li>
                    Meth Dealer (2018 - 2020)
                    <br>
                    &emsp; Freelance
                </li>
            </ul>
            </Section>
            <Section iconData={cogs} title="Skills">
                <ul>
                    <li><span>Meth Cooking</span>
                        <div class="gauge">
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                        </div>
                    </li>
                    <li>
                        <span>Quantum Physics Mastery</span>
                        <div class="gauge">
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet"></div>
                        </div>
                    </li>
                    <li>
                        <span>General Rizz</span>
                        <div class="gauge">
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet filled-bullet"></div>
                            <div class="bullet"></div>
                            <div class="bullet"></div>
                        </div>
                    </li>
                </ul>
            </Section>
        </div>
    </div>
    <a href="/">Return to Main Page</a><br>
</div>

<style>
h1 {
    font-family: "peralta";
}

ul {
    list-style-type: none;
}

li {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

li span {
    margin-right: 16px;
}

.gauge {
    display: flex;
    flex-direction: row;
}

.bullet {
    border-radius: 100%;
    width: 16px;
    height: 16px;
    margin: 4px;
    background-color: #fff59d;
}

.filled-bullet {
    background-color: #fbc02d;
}

.header-text {
    text-align: center;
    flex: 1;
    margin-right: 16px;
    color: #000000;
}

.readable-area {
    display: flex;
    flex-direction: column;
    background-color: #ffffff;
    margin: 0 15%;
    height: 100%;
}

.header {
    padding: 16px;
    display: flex;
    flex-direction: column-reverse;
    align-items: center;
    border-bottom: 2px solid black;
    text-decoration: none;
}



.content {
    display: grid;
    grid-template-columns: repeat(1, minmax(0,1fr));
    gap: 32px;
    padding: 32px;
}

.content-column {
    flex: 1;
    margin-top: 16px;
    padding: 0 16px 16px 16px;
    background-color: #ffffff;
}

img {
    width: 128px;
    height: 128px;
    padding: 4px;
    border: 4px solid #000000;
    border-radius: 100%;
}




i {
    background-color: transparent;
}



@media (min-width: 600px) {
    .header {
        flex-direction: row;
    }

    .header-text {
        text-align: end;
    }

    .content {
        grid-template-columns: repeat(2, minmax(0,1fr));   
    }

    .readable-area {
        margin: 0 10%;
    }
}

@media (min-width: 1000px) {
    .readable-area {
        margin: 0 20%;
    }
}
</style>